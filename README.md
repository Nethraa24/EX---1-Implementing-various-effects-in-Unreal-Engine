# EX-1 Implementing various effects in Unreal Engine

## Aim:
To implement various effects in a material such as emissive, roughness, and metallic properties in Unreal Engine.

## Procedure:
1. Open Unreal Engine and go to the Content Browser.
2. Right-click in the Content Browser and choose Material to create a new material asset.
3. Name the material (e.g., M_CustomEffect).
4. Double-click the material to open it in the Material Editor.
5. In the Material Editor, locate the Main Material Node (usually in the center).
6. For Base Color:

   - Add a Constant3Vector node (3-vector or use the shortcut 3) for color input.
   
   - Set the color and connect it to the Base Color input of the main node.
   
8. For Emissive Effect:

   - Add a Constant3Vector node and choose a bright color.

   - Add a Multiply node.

   - Connect the color to A and a Constant (e.g., value 10) to B.

   - Connect the Multiply output to the Emissive Color input.

10. For Roughness Control:

   - Add a Constant or Scalar Parameter (if you want it adjustable later).
   
   - Set value between 0 (smooth) and 1 (rough).
   
   - Connect it to the Roughness input of the material.

12. For Metallic Effect:

    - Add a Constant or Scalar Parameter node.

    - Set value to 0 for non-metal, 1 for full metal.

    - Connect it to the Metallic input.

14. Optional:

    - Add Texture Sample nodes for any map inputs (e.g., roughness map, metallic map).

    - Connect them to corresponding inputs (Roughness, Metallic, Emissive).

16. Change the Material Blend Mode to Opaque (or others as needed).
17. Click Apply and Save the material.
18. Go to the Viewport, select a mesh or surface.
19. Drag and drop your material onto the mesh or apply it via the Details Panel.


## Output:
### For Emissive Effect:
![WhatsApp Image 2025-05-08 at 13 36 35_52c2bafd](https://github.com/user-attachments/assets/1f77fc8c-3835-4a9a-9492-292a958dd835)


### For Roughness Control:
![WhatsApp Image 2025-05-08 at 13 36 36_e35a6ee4](https://github.com/user-attachments/assets/a9951230-4d17-499d-9a48-5c4499ae87ce)


### For Metallic Effect:

![WhatsApp Image 2025-05-08 at 13 38 19_002648e1](https://github.com/user-attachments/assets/dd953379-8e2d-45d0-b32e-4326cfe3280b)


## Result:
A custom material is successfully created and applied, displaying realistic or stylized emissive lighting, surface roughness, and metallic properties in Unreal Engine.

