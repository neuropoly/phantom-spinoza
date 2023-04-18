# phantom-spinoza

CAD model and recipe for MRI head-torso phantom fabrication

<img width="600" alt="image" src="https://user-images.githubusercontent.com/2482071/218195449-e91c9f69-b2c5-46ff-ad4c-8ceca5081e5f.png">

## Citation

> Rios NL, Gilbert KM, Papp D, Cereza G, Foias A, Rangaprakash D, May MW, Guerin B, Wald LL, Keil B, Stockmann JP, Barry RL, Cohen-Adad J. 8-channel Tx dipole and 20-channel Rx loop coil array for MRI of the cervical spinal cord at 7 Tesla [Internet]. 2023. Available from: http://biorxiv.org/lookup/doi/10.1101/2023.02.08.527664

## Recipe

Phantom physical characteristics:
- Inner volume: 14.156 L
- Total phantom weight: 16.257 kg

Ingredients:
- Water (demineralized): 9,900 mL
- Mouthwash (no alcohol): 600 mL (~4% of final volume)
- Salt: 254 g
- Sugar: 7,913 g
- Agar: 116g (0.75% of final volume)

<details><summary>Permittivity, conductivity and details about the ingredients</summary>

The recipe was based on [this website](https://amri.ninds.nih.gov/cgi-bin/phantomrecipe): 

<img width="400" alt="image" src="https://user-images.githubusercontent.com/2482071/218194541-e70796ac-888b-4f0d-938a-c0b9493f01b1.png">
<img width="400" alt="image" src="https://user-images.githubusercontent.com/2482071/218194552-76b2efde-d5aa-4177-8b61-b956b3651892.png">

</details>

> **Note**
> The mouthwash amount (600 mL) is included in the estimated water volume (10,500ml). Mouthwash is used to prevent the growth of bacteria that is likely to occur in a mixture containing sugar and agar. It was assumed that the efficacy of an alcohol-based mouthwash would be reduced due to the rapid evaporation of the alcohol portion during the mixing process due to the high temperature required. For this reason, an alcohol-free mouthwash was selected. 

<img width="600" alt="image" src="https://user-images.githubusercontent.com/2482071/218194874-fe055065-314a-4f54-a4bf-cb6dfae6ce48.png">

## Parameters (@3T)

- Conductivity: 0.74 S/m
- Permittivity: 68.5
- T1: ~500 ms
- T2: ~50 ms
- T2*: ~10 ms

## Parameters (@7T)

- Conductivity: 0.78 S/m
- Permittivity: 63.3

> **Note**
> Our goal was to obtain a mixture that mimicked the average human tissue in the region of interest in terms of dielectric parameters and relaxation times. To do this, we had to find a trade-off between [sugar](https://aapm.onlinelibrary.wiley.com/doi/abs/10.1118/1.4895823) and [agar](https://aapm.onlinelibrary.wiley.com/doi/full/10.1118/1.3656077) concentrations, since both affect relaxation times, and sugar is used to control permittivity. This allowed us to keep the permittivity and relaxation times within the range of human tissues while still producing a gel.

## Tips

Phantom shell construction:
- Description: The phantom shell was divided in two parts for 3D printing to provide a hole of 110mm in diameter at the top of the head. This opening is needed to manually remove 3D-printed supports and finish the inner surface by sanding and waterproofing. The shell has also a D-shaped filling hole on one side where a PVC reducing bushing (Schedule 40 ¾ spigot X ½ FTP) is manually D-shaped and glued. After filling the phantom, the bushing is closed with a PVC plug (Schedule 40 ½ MPT).
- Printing material: PLA 2.0 EcoTough™
- Printer: Modix BIG-60
- Printing parameters: [NeckPhantom6](https://github.com/neuropoly/phantom-spinoza/blob/main/NeckPhantom6.curaprofile). 
- Remove all 3D-printing supports and residues from all surfaces.
- Smooth all surfaces carefully with sandpaper (120 and 220 grit).
- Waterproof inner surfaces by coating it with epoxy (e.g., Smooth-On, XTC-3D™). 
- After the inner surfaces of both parts are completely coated and dry, assemble the shell: glue or (plastic) weld its two sections and glue the PVC bushing. Use epoxy for gluing (J-B WELD, High Strength Plastic Bonder, Adhesive Syringe - Tan, 25 ml).
- Reinforce exterior surfaces with epoxy (e.g., Smooth-On, XTC-3D™) and fiberglass (#120-38 Standard E-Glass Fiberglass Cloth). The fiberglass provides the phantom with additional resistance to moderate impacts. This [video](https://www.youtube.com/watch?v=ioj1YBm6bJY) shows how to select the fiberglass and [this one](https://www.youtube.com/watch?v=ujk-wBQDUSk) describes how to apply it. 
- The fiberglass chosen is flexible, easy to work with, inexpensive, and strong enough for this application. Note that the Phantom is heavy when fully loaded (17kg) and a strong impact such as a drop will likely render the shell useless, even if a stronger and more expensive reinforcing material such as carbon fiber is used.
- Thoroughly clean the interior of the coated shell and test it for waterproofness by filling it with water and inspecting it after 24 hours.

Mixture preparation:
- Ensure that no contaminating particles can fall into the mixture.
- Place large container (20 liters) on a [hot plate](https://www.hubert.ca/product/75300/Cadco-CSR-3T-Stainless-Steel-Single-Burner-Hot-Plate-With-8Dia-Element---12-14L-x-14W-x-4-18W) and add water. A [hot pot with a faucet](https://www.homedepot.ca/product/camp-chef-19l-20-qt-aluminum-hot-water-pot/1001156780) is recommended.
- Turn the hot plate on and wait for temperature to reach 60deg.
- Start stirring and do not stop during the whole process. Avoid splashing. 
- Add salt and dissolve it.
- Add sugar gradually, dissolving each portion.
- Add agar when the temperature has reached 90 deg and dissolve it.
- Turn hot plate off. Continue stirring. 
- Add mouthwash and stir for a few minutes to homogenize the mixture. 
- Continue stirring for some time to prevent the mixture from burning at the bottom of the container.
- Wait for temp to reach 60 deg to to facilitate the release of air bubbles.
- Pour the mixture into the phantom avoiding bubbles. To do this, a hose connected to the pot's faucet and passing through the phantom inlet can be used to drive the mixture flow directly to one of the inner surfaces of the shell, as is done to fill a glass of beer.

