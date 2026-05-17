# 3D CT Image Visualization using Blender

This project presents a reusable CT visualization workflow developed in Blender using Bioxel Nodes.

The workflow enables automated rendering and color mapping of volumetric CT datasets through reusable node-based templates.

---

## Features

- Node-based visualization pipeline
- Reusable Blender templates
- Soft tissue visualization
- Brain structure visualization
- Adjustable rendering parameters
- Slice-based exploration using plane cutters

---

## Software

- Blender
- Bioxel Nodes

---

## Workflow

<p align="center">
  <img src="renders/pipeline.png" width="75%">
</p>

<p align="center">
  <em>Overview of the reusable visualization workflow developed in Blender using Bioxel Nodes.</em>
</p>

---

## Example Results

### Soft Tissue Visualization

<p align="center">
  <img src="renders/Soft_tissue.png" width="43.5%">
  <img src="renders/Soft_tissue_slide.png" width="45%">
</p>

<p align="center">
  <em>Soft tissue visualization with and without sectional slicing.</em>
</p>

---

### Brain Structure Visualization

<p align="center">
  <img src="renders/Brain.png" width="45%">
  <img src="renders/Brain_slide.png" width="45%">
</p>

<p align="center">
  <em>Brain-oriented visualization showing internal structures and slice-based exploration.</em>
</p>
---

## Blender Templates

- `brain_visualization_template.blend`
- `soft_tissue_visualization_template.blend`

These templates contain predefined node structures, rendering parameters, and visualization settings for reusable CT visualization workflows.

---

# Usage

## Opening the Template

1. Open Blender.
2. Open one of the provided template files:

   * `brain_visualization_template.blend`
   * `soft_tissue_visualization_template.blend`

The templates already contain:

* predefined Bioxel Nodes workflows
* rendering settings
* lighting setup
* slicing tools
* visualization parameters

---

## Importing a CT Dataset

1. Install the Bioxel Nodes add-on in Blender.
2. In Blender, open the Bioxel Nodes panel.
3. Import a CT dataset (DICOM, NIfTI, or supported volumetric format).
4. The dataset will be loaded as a volumetric object.

After importing, the predefined node workflow can be connected directly to the imported volume.

---

## Reusing the Workflow with Append

The visualization pipeline can also be reused in other Blender projects using Blender's Append function.

### Append the Node Template

1. Open your Blender project.
2. Go to:

```text
File → Append
```

3. Select one of the template `.blend` files.
4. Open:

```text
NodeTree
```

or

```text
GeometryNodeTree
```

5. Select the desired node group.
6. Click:

```text
Append
```

The node workflow will now be available in the current Blender project.

---

## Rendering

1. Connect the imported CT volume to the node workflow.
2. Adjust threshold or color parameters if needed.
3. Use the predefined camera and lighting setup.
4. Render the scene using Cycles.

---

## Example Workflow

```text
Import CT Data
        ↓
Connect to Template
        ↓
Adjust Threshold / Color
        ↓
Render Visualization
```

---

## Notes

* The templates are designed for reusable scientific visualization workflows.
* Different visualization styles can be achieved by modifying threshold ranges, opacity, and color mapping.
* For best compatibility, use Blender together with the latest version of Bioxel Nodes.

## Author

Shen Gao
