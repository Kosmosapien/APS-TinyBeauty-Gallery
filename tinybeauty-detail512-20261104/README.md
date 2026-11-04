# TinyBeauty — Microtextura em 512 × 512

Galeria alternativa para celular, sem depender da publicação do GitHub Pages.

Compare o teacher corrigido com a saída da U-Net de 256 pixels ampliada,
a aplicação do residual sobre a imagem 512 e o refinador de alta frequência.
O TinyBeauty sem Albumentations continua preservado como MVP.

**Nota metodológica:** energia espectral próxima da do teacher não significa textura correta.
A variante de microcontraste pode produzir detalhes diferentes dos desejados.

[Abrir a galeria interativa, quando disponível](https://kosmosapien.github.io/APS-TinyBeauty-Gallery/tinybeauty-detail512-20261104/)

### Comparação de modelos (136 identidades de validação)

| Versão | Erro highpass (↓) | Energia highpass relativa ao teacher |
|:--|--:|--:|
| U-Net 256 ampliada, RGB inteiro | 0,02284 | 55,4% |
| Residual da U-Net sobre fotografia original 512 | 0,02688 | 88,2% |
| Refinador 512, perda pixelwise | 0,02213 | 45,8% |
| Refinador 512, perda de altas frequências | **0,02202** | 45,5% |
| Refinador 512, perda de microcontraste | 0,02792 | **98,2%** |

### Fotografias de validação

Clique para expandir cada identidade. Todas as versões têm a mesma fonte e o mesmo teacher.

<details>
<summary><strong>Identidade 01</strong> — SFHQ_pt3_00001690</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/01_original.webp" alt="Original 01" width="270">
<img src="assets/01_teacher.webp" alt="Teacher 01" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/01_whole_rgb_up.webp" alt="Ampliação RGB 01" width="270">
<img src="assets/01_residual_up.webp" alt="Residual aplicado a original 01" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/01_pixel_02500.webp" alt="Controle pixel 01" width="210">
<img src="assets/01_frequency_02500.webp" alt="Controle frequência 01" width="210">
<img src="assets/01_energy_02500.webp" alt="Microcontraste 01" width="210">

</details>

<details>
<summary><strong>Identidade 02</strong> — SFHQ_pt3_00002799</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/02_original.webp" alt="Original 02" width="270">
<img src="assets/02_teacher.webp" alt="Teacher 02" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/02_whole_rgb_up.webp" alt="Ampliação RGB 02" width="270">
<img src="assets/02_residual_up.webp" alt="Residual aplicado a original 02" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/02_pixel_02500.webp" alt="Controle pixel 02" width="210">
<img src="assets/02_frequency_02500.webp" alt="Controle frequência 02" width="210">
<img src="assets/02_energy_02500.webp" alt="Microcontraste 02" width="210">

</details>

<details>
<summary><strong>Identidade 03</strong> — SFHQ_pt3_00005043</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/03_original.webp" alt="Original 03" width="270">
<img src="assets/03_teacher.webp" alt="Teacher 03" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/03_whole_rgb_up.webp" alt="Ampliação RGB 03" width="270">
<img src="assets/03_residual_up.webp" alt="Residual aplicado a original 03" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/03_pixel_02500.webp" alt="Controle pixel 03" width="210">
<img src="assets/03_frequency_02500.webp" alt="Controle frequência 03" width="210">
<img src="assets/03_energy_02500.webp" alt="Microcontraste 03" width="210">

</details>

<details>
<summary><strong>Identidade 04</strong> — SFHQ_pt3_00005983</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/04_original.webp" alt="Original 04" width="270">
<img src="assets/04_teacher.webp" alt="Teacher 04" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/04_whole_rgb_up.webp" alt="Ampliação RGB 04" width="270">
<img src="assets/04_residual_up.webp" alt="Residual aplicado a original 04" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/04_pixel_02500.webp" alt="Controle pixel 04" width="210">
<img src="assets/04_frequency_02500.webp" alt="Controle frequência 04" width="210">
<img src="assets/04_energy_02500.webp" alt="Microcontraste 04" width="210">

</details>

<details>
<summary><strong>Identidade 05</strong> — SFHQ_pt3_00006549</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/05_original.webp" alt="Original 05" width="270">
<img src="assets/05_teacher.webp" alt="Teacher 05" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/05_whole_rgb_up.webp" alt="Ampliação RGB 05" width="270">
<img src="assets/05_residual_up.webp" alt="Residual aplicado a original 05" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/05_pixel_02500.webp" alt="Controle pixel 05" width="210">
<img src="assets/05_frequency_02500.webp" alt="Controle frequência 05" width="210">
<img src="assets/05_energy_02500.webp" alt="Microcontraste 05" width="210">

</details>

<details>
<summary><strong>Identidade 06</strong> — SFHQ_pt3_00006969</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/06_original.webp" alt="Original 06" width="270">
<img src="assets/06_teacher.webp" alt="Teacher 06" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/06_whole_rgb_up.webp" alt="Ampliação RGB 06" width="270">
<img src="assets/06_residual_up.webp" alt="Residual aplicado a original 06" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/06_pixel_02500.webp" alt="Controle pixel 06" width="210">
<img src="assets/06_frequency_02500.webp" alt="Controle frequência 06" width="210">
<img src="assets/06_energy_02500.webp" alt="Microcontraste 06" width="210">

</details>

<details>
<summary><strong>Identidade 07</strong> — SFHQ_pt3_00007250</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/07_original.webp" alt="Original 07" width="270">
<img src="assets/07_teacher.webp" alt="Teacher 07" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/07_whole_rgb_up.webp" alt="Ampliação RGB 07" width="270">
<img src="assets/07_residual_up.webp" alt="Residual aplicado a original 07" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/07_pixel_02500.webp" alt="Controle pixel 07" width="210">
<img src="assets/07_frequency_02500.webp" alt="Controle frequência 07" width="210">
<img src="assets/07_energy_02500.webp" alt="Microcontraste 07" width="210">

</details>

<details>
<summary><strong>Identidade 08</strong> — SFHQ_pt3_00007369</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/08_original.webp" alt="Original 08" width="270">
<img src="assets/08_teacher.webp" alt="Teacher 08" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/08_whole_rgb_up.webp" alt="Ampliação RGB 08" width="270">
<img src="assets/08_residual_up.webp" alt="Residual aplicado a original 08" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/08_pixel_02500.webp" alt="Controle pixel 08" width="210">
<img src="assets/08_frequency_02500.webp" alt="Controle frequência 08" width="210">
<img src="assets/08_energy_02500.webp" alt="Microcontraste 08" width="210">

</details>

<details>
<summary><strong>Identidade 09</strong> — SFHQ_pt3_00007455</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/09_original.webp" alt="Original 09" width="270">
<img src="assets/09_teacher.webp" alt="Teacher 09" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/09_whole_rgb_up.webp" alt="Ampliação RGB 09" width="270">
<img src="assets/09_residual_up.webp" alt="Residual aplicado a original 09" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/09_pixel_02500.webp" alt="Controle pixel 09" width="210">
<img src="assets/09_frequency_02500.webp" alt="Controle frequência 09" width="210">
<img src="assets/09_energy_02500.webp" alt="Microcontraste 09" width="210">

</details>

<details>
<summary><strong>Identidade 10</strong> — SFHQ_pt3_00008011</summary>

<p><strong>Original / Teacher:</strong></p>
<img src="assets/10_original.webp" alt="Original 10" width="270">
<img src="assets/10_teacher.webp" alt="Teacher 10" width="270">

<p><strong>U-Net RGB ampliada / Transformação residual em 512:</strong></p>
<img src="assets/10_whole_rgb_up.webp" alt="Ampliação RGB 10" width="270">
<img src="assets/10_residual_up.webp" alt="Residual aplicado a original 10" width="270">

<p><strong>Refinador pixel / Frequência / Microcontraste — 2500 passos:</strong></p>
<img src="assets/10_pixel_02500.webp" alt="Controle pixel 10" width="210">
<img src="assets/10_frequency_02500.webp" alt="Controle frequência 10" width="210">
<img src="assets/10_energy_02500.webp" alt="Microcontraste 10" width="210">

</details>

## Arquivos e reprodução

Dataset de validação: 136 identidades V4 Social corrigido; treino 1000 pares.
Scripts e pesos estão em NeuralFilters e C:\Datasets\APS-Makeup\TinyBeautyExperiments\Global512Detail_20261104.
Nenhuma versão foi promovida ao MVP; resultados para avaliação e pesquisa.
