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

🔗 [Odin3 v3.13.3](https://samfw.com/Odin/Odin3_v3.13.3.zip)

Extraia o arquivo e faça o flash da firmware INS no dispositivo.

> ⚠️ **Atenção:** o processo de instalação da firmware pode apagar os dados do aparelho. Tenha seu backup pronto antes de continuar.

Depois que o flash terminar, configure o aparelho normalmente.

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

🔗 [Odin3 v3.13.3](https://samfw.com/Odin/Odin3_v3.13.3.zip)

Extract the file and flash the INS firmware onto the device.

> ⚠️ **Warning:** The firmware installation process may erase the device. Make sure you have a backup before continuing.

After the flash is complete, set up the device normally.

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
