# Tips 1
<details>
<summary>next</summary>

長くなるなら折りたたみ

## Code
  
```glsl
float move = 12.5;
float line = smoothstep(0.995, 1.0, sin(vUv.x * 50.0 * aspect + 1.0 + normal.x * move * aspect));
line += smoothstep(0.995, 1.0, sin(vUv.y * 50.0 + 1.0 + normal.y * move));
line = clamp(line, 0.0, 1.0);
color = mix(color * 0.92, color, 1.0 - line);
```
<img src='https://github.com/nemutas/readme-test/assets/46724121/f4303e75-5380-4523-9e17-f30d274d818c' width='700' />

</details>

# Tips 2
長くならないなら、べた書き<br />
https://www.youtube.com/live/0D-J_Lbxeeg?si=ZtCf4NX9VhojGIfX
