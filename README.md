# 📱 Samsung Galaxy A36 5G — One UI Beta via INS Region

> 🇧🇷 **Português abaixo · English below**

---

# 🇧🇷 Português (PT-BR)

## 📱 Como receber a Beta da One UI usando a região INS

> ⚠️ **IMPORTANTE:** Este procedimento foi **testado somente no Samsung Galaxy A36 5G SM-A366E**.
> Não há garantia de que funcione em outros modelos ou variantes.

Este tutorial ensina como instalar a **Stock ROM INS (Índia)** no Galaxy A36 5G SM-A366E e alterar a região do dispositivo para tentar receber uma atualização Beta da One UI através do Samsung Members.

## ⚠️ Avisos importantes

* 🔴 **Este processo foi testado somente no SM-A366E.**
* 💾 O processo de flash **formata o dispositivo**. Faça um backup de todos os seus arquivos antes de começar.
* 🔌 Use um **cabo USB de boa qualidade**.
* 💻 Recomendo utilizar um computador para realizar o procedimento.
* 📱 É possível realizar o flash pelo celular, mas **este tutorial não aborda esse método**.
* 🔋 Certifique-se de que o dispositivo tenha bateria suficiente antes de começar.
* ⚠️ Faça tudo por sua própria conta e risco.

> **Disclaimer:** Não me responsabilizo por qualquer dano causado durante o procedimento.
> Seu dispositivo pode simplesmente funcionar normalmente, pode dar algum problema, pode morrer, ou, em casos extremamente criativos, criar pernas e fugir de você. 🏃📱

---

## 🚀 Tutorial

### 1. Baixe a firmware INS

Baixe a **Stock ROM da Índia (INS)** correspondente ao **SM-A366E**.

🔗 [Download da firmware INS — SamFW](https://samfw.com/firmware/SM-A366E/INS)

> ⚠️ Confira cuidadosamente o modelo antes de baixar ou instalar qualquer arquivo.

---

### 2. Faça o flash da firmware usando Odin

Baixe o Odin:

🔗 [Odin3 v3.13.3 — SamFW](https://samfw.com/Odin/Odin3_v3.13.3.zip)

Extraia o arquivo do Odin e também o `.zip` da firmware INS.

#### 2.1 Entre no Modo de Manutenção

Antes de entrar no Download Mode, o dispositivo precisa estar **desligado e em Modo de Manutenção**.

Para entrar no Modo de Manutenção:

1. Abra **Configurações**.
2. Acesse **Assistência do aparelho**.
3. Procure pela opção **Modo de Manutenção**.
4. Ative o **Modo de Manutenção**.
5. Aguarde o processo terminar.
6. Certifique-se de que o aparelho esteja desligado antes de continuar.

#### 2.2 Entre no Download Mode

Com o dispositivo desligado:

1. Segure **Volume + e Volume - simultaneamente**.
2. Enquanto mantém os dois botões pressionados, conecte o cabo USB ao computador.
3. O dispositivo deverá entrar no **Download Mode**.
4. Confirme a entrada no Download Mode quando solicitado pelo aparelho.

> ⚠️ **Não desconecte o cabo USB durante o processo de flash.**

---

#### 2.3 Abra o Odin

Abra o **Odin** no computador.

Quando o dispositivo for reconhecido, o Odin deverá mostrar uma porta indicando que o aparelho foi conectado.

Agora extraia a firmware INS.

Dentro dela estarão os arquivos necessários para o flash.

No Odin, selecione os arquivos correspondentes:

| Campo no Odin | Arquivo                      |
| ------------- | ---------------------------- |
| **BL**        | Arquivo que começa com `BL_` |
| **AP**        | Arquivo que começa com `AP_` |
| **CP**        | Arquivo que começa com `CP_` |
| **CSC**       | Arquivo `CSC_ODM_`           |

> 🚨 **IMPORTANTE:** No campo **CSC**, selecione o arquivo **`CSC_ODM`** e **NÃO** selecione o `HOME_CSC_ODM`.

O `CSC_ODM` será utilizado para realizar uma instalação limpa da firmware e, consequentemente, **apagar os dados do dispositivo**.

O `HOME_CSC_ODM` **não deve ser utilizado neste tutorial**.

---

#### 2.4 Inicie o flash

Antes de iniciar, confira novamente:

* **BL** → `BL_...`
* **AP** → `AP_...`
* **CP** → `CP_...`
* **CSC** → `CSC_ODM_...`

Certifique-se de que todos os arquivos pertencem à **mesma firmware INS**.

Depois:

1. Confirme que o Odin reconheceu o dispositivo.
2. Confirme que o campo **CSC** está usando `CSC_ODM`.
3. Clique em **Start**.
4. Aguarde o processo terminar.

> ⚠️ **NÃO desconecte o cabo USB durante o flash.**
>
> ⚠️ **NÃO desligue o computador.**
>
> ⚠️ **NÃO tente mexer no aparelho enquanto o Odin estiver realizando o processo.**

Quando o processo terminar, o Odin deverá mostrar:

```text
PASS!
```

O dispositivo será reiniciado automaticamente.

Depois que o aparelho iniciar, faça a configuração inicial normalmente.

> 💾 Como foi utilizado o `CSC_ODM` em vez do `HOME_CSC_ODM`, o dispositivo será formatado. É normal que os dados anteriores não estejam mais presentes.

---

### 3. Instale o Samsung Region Override e o Shizuku

Baixe os aplicativos necessários:

* 🔧 [Samsung Region Override](https://github.com/Ritel-T/SamsungRegionOverride)
* 🛠️ [Shizuku](https://github.com/thedjchi/Shizuku)

Instale ambos no Galaxy A36.

---

### 4. Configure o Shizuku

Abra o **Shizuku** e inicie o serviço utilizando **Depuração sem fio (Wireless Debugging)**.

Depois que o Shizuku estiver funcionando:

1. Abra o Samsung Region Override.
2. Quando solicitado, conceda a permissão do Shizuku.
3. Verifique se o Samsung Region Override consegue acessar o serviço.

---

### 5. Altere a região para Índia 🇮🇳

Abra o **Samsung Region Override**.

Altere a região do dispositivo para:

```text
India
```

ou para o código de região correspondente à Índia, quando solicitado pelo aplicativo.

> ℹ️ O objetivo desta etapa é fazer com que os serviços da Samsung reconheçam o dispositivo como pertencente à região da Índia.

---

### 6. Faça login na sua Samsung Account

Entre com sua **Samsung Account** no dispositivo.

Certifique-se de que a conta esteja corretamente configurada antes de continuar.

---

### 7. Abra o Samsung Members

Abra o aplicativo **Samsung Members**.

Role a página inicial até o final e procure pelo banner referente ao **programa Beta da One UI**.

> ⚠️ A disponibilidade do banner depende da Samsung, da região, do modelo e do período em que o programa Beta estiver aberto.

---

### 8. Entre no programa Beta

Caso o banner esteja disponível:

1. Toque no banner do programa Beta.
2. Leia os termos apresentados.
3. Faça a inscrição no programa Beta.

Depois disso, aguarde o registro ser processado.

---

### 9. Procure por atualizações

Agora vá para:

**Configurações → Atualização de software → Baixar e instalar**

Toque para procurar uma nova atualização.

Se o dispositivo tiver sido aceito no programa Beta e a atualização estiver disponível para sua variante, ela deverá aparecer aqui.

---

### 🎉 10. Pronto!

Se tudo deu certo, basta:

1. Baixar a atualização.
2. Instalar.
3. Aguardar o aparelho reiniciar.
4. Aproveitar a nova versão da One UI. 🚀

---

## ⚠️ Considerações finais

Este tutorial documenta um procedimento que foi **testado somente no SM-A366E**.

Não tente aplicar este procedimento cegamente em outros modelos, variantes ou firmwares. A Samsung tem uma quantidade gloriosa de variantes com nomes quase idênticos, porque aparentemente facilitar a vida do usuário seria uma feature paga. 💀

**Use por sua própria conta e risco e mantenha sempre um backup dos seus dados.**

---

# 🇺🇸 English

## 📱 How to Receive the One UI Beta Using the INS Region

> ⚠️ **IMPORTANT:** This procedure was **only tested on the Samsung Galaxy A36 5G SM-A366E**.
> There is no guarantee that it will work on other models or variants.

This tutorial explains how to install the **INS (India) Stock ROM** on the Galaxy A36 5G SM-A366E and change the device region in an attempt to receive a One UI Beta update through Samsung Members.

## ⚠️ Important warnings

* 🔴 **This procedure was only tested on the SM-A366E.**
* 💾 The flashing process **will factory reset the device**. Back up all your files before starting.
* 🔌 Use a **good-quality USB cable**.
* 💻 A computer is recommended for this procedure.
* 📱 It is possible to flash from a phone, but **this tutorial does not cover that method**.
* 🔋 Make sure your device has enough battery before starting.
* ⚠️ Perform this procedure at your own risk.

> **Disclaimer:** I am not responsible for any damage caused during this procedure.
> Your device may work perfectly, it may encounter problems, it may die, or, in particularly creative circumstances, grow legs and run away from you. 🏃📱

---

## 🚀 Tutorial

### 1. Download the INS firmware

Download the **India (INS) Stock ROM** corresponding to the **SM-A366E**.

🔗 [Download INS firmware — SamFW](https://samfw.com/firmware/SM-A366E/INS)

> ⚠️ Carefully verify the model before downloading or installing any firmware.

---

### 2. Flash the firmware using Odin

Download Odin:

🔗 [Odin3 v3.13.3 — SamFW](https://samfw.com/Odin/Odin3_v3.13.3.zip)

Extract the Odin file and the INS firmware `.zip`.

#### 2.1 Enter Maintenance Mode

Before entering Download Mode, the device needs to be **powered off and in Maintenance Mode**.

To enter Maintenance Mode:

1. Open **Settings**.
2. Go to **Device care**.
3. Look for the **Maintenance Mode** option.
4. Enable **Maintenance Mode**.
5. Wait for the process to finish.
6. Make sure the device is powered off before continuing.

#### 2.2 Enter Download Mode

With the device powered off:

1. Hold **Volume Up and Volume Down simultaneously**.
2. While holding both buttons, connect the USB cable to the computer.
3. The device should enter **Download Mode**.
4. Confirm entering Download Mode when prompted by the device.

> ⚠️ **Do not disconnect the USB cable during the flashing process.**

---

#### 2.3 Open Odin

Open **Odin** on your computer.

Once the device is detected, Odin should display a port indicating that the device has been connected.

Now extract the INS firmware.

Inside the firmware package you will find the files required for flashing.

Select the corresponding files in Odin:

| Odin field | File                     |
| ---------- | ------------------------ |
| **BL**     | File starting with `BL_` |
| **AP**     | File starting with `AP_` |
| **CP**     | File starting with `CP_` |
| **CSC**    | `CSC_ODM_` file          |

> 🚨 **IMPORTANT:** In the **CSC** field, select the **`CSC_ODM`** file and **DO NOT** select `HOME_CSC_ODM`.

`CSC_ODM` is used to perform a clean firmware installation and will therefore **erase the device data**.

`HOME_CSC_ODM` **should not be used in this tutorial**.

---

#### 2.4 Start the flash

Before starting, check everything again:

* **BL** → `BL_...`
* **AP** → `AP_...`
* **CP** → `CP_...`
* **CSC** → `CSC_ODM_...`

Make sure all files belong to the **same INS firmware**.

Then:

1. Confirm that Odin has detected the device.
2. Confirm that the **CSC** field is using `CSC_ODM`.
3. Click **Start**.
4. Wait for the process to finish.

> ⚠️ **DO NOT disconnect the USB cable during the flash.**
>
> ⚠️ **DO NOT turn off the computer.**
>
> ⚠️ **DO NOT interfere with the device while Odin is flashing.**

When the process is complete, Odin should display:

```text
PASS!
```

The device will reboot automatically.

After the device starts, complete the initial setup normally.

> 💾 Since `CSC_ODM` was used instead of `HOME_CSC_ODM`, the device will be factory reset. It is normal for your previous data to be gone.

---

### 3. Install Samsung Region Override and Shizuku

Download the required applications:

* 🔧 [Samsung Region Override](https://github.com/Ritel-T/SamsungRegionOverride)
* 🛠️ [Shizuku](https://github.com/thedjchi/Shizuku)

Install both applications on your Galaxy A36.

---

### 4. Set up Shizuku

Open **Shizuku** and start the service using **Wireless Debugging**.

Once Shizuku is running:

1. Open Samsung Region Override.
2. Grant the Shizuku permission when prompted.
3. Make sure Samsung Region Override can access the Shizuku service.

---

### 5. Change the region to India 🇮🇳

Open **Samsung Region Override**.

Change the device region to:

```text
India
```

or use the corresponding India region code if requested by the application.

> ℹ️ The purpose of this step is to make Samsung services recognize the device as belonging to the Indian region.

---

### 6. Sign in to your Samsung Account

Sign in to your **Samsung Account** on the device.

Make sure the account is properly configured before continuing.

---

### 7. Open Samsung Members

Open the **Samsung Members** application.

Scroll down through the home page and look for the **One UI Beta** program banner.

> ⚠️ Banner availability depends on Samsung, the region, the device model, and whether the Beta program is currently open.

---

### 8. Join the Beta program

If the Beta banner is available:

1. Tap the Beta program banner.
2. Read the provided terms.
3. Enroll in the Beta program.

Wait for the enrollment to be processed.

---

### 9. Check for updates

Go to:

**Settings → Software update → Download and install**

Tap to check for a new update.

If the device has been accepted into the Beta program and the update is available for your variant, it should appear here.

---

### 🎉 10. Done!

If everything worked:

1. Download the update.
2. Install it.
3. Wait for the device to reboot.
4. Enjoy the new One UI version. 🚀

---

## ⚠️ Final notes

This tutorial documents a procedure that was **only tested on the SM-A366E**.

Do not blindly apply this procedure to other models, variants, or firmware versions. Samsung has a glorious collection of nearly identical variants, because apparently making things easy for users would be a paid feature. 💀

**Use this guide at your own risk and always keep a backup of your data.**
