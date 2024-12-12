---
title: DocumentExtensions
layout: page
---

**Summary:** Provides extension methods for the Autodesk Revit API.

## Methods

### GetFamilyTypesByCategoryOrderedByName(Autodesk.Revit.DB.Document,Autodesk.Revit.DB.BuiltInCategory)

**Summary:** Retrieves all family types of the specified category from the given Revit document as an ObservableCollection.

#### Parameters:
- `doc`: The Revit document to search for family types.
- `category`: The BuiltInCategory to filter family types.

#### Returns:
An ObservableCollection containing all FamilySymbol objects representing the specified category.

---

### GetLevelsOrderedByProperty``1(Autodesk.Revit.DB.Document,System.Func{Autodesk.Revit.DB.Level,``0},System.Boolean)

**Summary:** Retrieves all levels from the specified Revit document as an ObservableCollection,
            with dynamic ordering based on a specified property.

#### Parameters:
- `doc`: The Revit document to search for levels.
- `keySelector`: A function to extract a key from a Level for ordering.
- `ascending`: If true, orders levels in ascending order; otherwise, descending.

#### Returns:
An ObservableCollection containing Level objects, ordered dynamically by the specified property.

---

### GetRebarShapes(Autodesk.Revit.DB.Document)

**Summary:** Retrieves all rebar shapes from the specified Revit document.

#### Parameters:
- `doc`: The Revit document to retrieve rebar shapes from.

#### Returns:
A list of RebarShape objects available in the document.

---

### GetRebarBarTypes(Autodesk.Revit.DB.Document)

**Summary:** Retrieves all rebar bar types from the specified Revit document as an ObservableCollection.

#### Parameters:
- `doc`: The Revit document to retrieve rebar bar types from.

#### Returns:
An ObservableCollection containing all RebarBarType objects in the document.

---

### CreateAndPlaceColumnAtPoint(Autodesk.Revit.DB.Document,Autodesk.Revit.DB.XYZ,Autodesk.Revit.DB.FamilySymbol,Autodesk.Revit.DB.Level,Autodesk.Revit.DB.Level)

**Summary:** Prompts the user to select a point and places a column at that point.

#### Parameters:
- `doc`: The Revit document where the column will be placed.
- `point`: The XYZ point where the column will be placed.
- `columnType`: The FamilySymbol representing the column type.
- `baseLevel`: The base level of the column.
- `topLevel`: The top level of the column.

#### Returns:
The created column Element, or null if no column was created.

---

### SearchOrCreate3DView(Autodesk.Revit.DB.Document,System.String)

**Summary:** Searches for a 3D view with the specified name. If it exists, returns it. Otherwise, creates a new 3D view.

#### Parameters:
- `doc`: The Revit document to search or create the 3D view in.
- `viewName`: The name of the 3D view to search for or create.

#### Returns:
The existing or newly created View3D object.

---

