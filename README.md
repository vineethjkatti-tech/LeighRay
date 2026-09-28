# LeighRay

## Project Overview & Physics

Unlike traditional **magnetic compasses** which malfunction near laptops, cars and strong magnetic fields **LeighRay** uses a similar technique to that of Desert ants to determine the location of the sun. 

### Rayleigh Scattering

<img width="600" height="510" alt="image" src="https://github.com/user-attachments/assets/f6996ad5-7a69-4caa-bac5-bdd3edb59ddc" />

The compass uses **Rayleigh Light Scatters** - which is basically the sunlight scattered by the atmosphere to determine where the sun is. These rays are polarized along an electric field which is strictly **perpendicular** to the position of Sun.

### Stokes Parameter Derivation

By capturing the light intensity through four **linear polarizers** that are inclined at **0°**, **45°**, **90°** and **135°** respectively, the system extracts the **Stokes Parameters**

$$S_1 = I_0 - I_{90}, \quad S_2 = I_{45} - I_{135}$$


**Angle of Polarization**

$$\theta = \frac{1}{2} \text{atan2}(S_2, S_1)$$


**True North Lock**: The on-chip Platforme Solar de Almeria (PSA) calculates the sun's celestial **azimuth** (_the horizontal angle of a direction, measured clockwise from a reference direction like North on a scale from 0° to 360°_). Subtracting the relative sky vector yields the **true north** without the usage of any magnetism.


<img width="401" height="383" alt="image" src="https://github.com/user-attachments/assets/b6d8f8a7-2d7d-4dab-af42-15aba1abaf5d" />

