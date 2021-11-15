---
title: Informazioni sull'amministratore
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Questo articolo contiene le risposte alle domande frequenti relative alle informazioni sull'amministratore in Microsoft Forms.
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951486"
---
# <a name="admin-information"></a>Informazioni sull'amministratore

## <a name="getting-started"></a>Introduzione

**Come si disattiva o si attiva Microsoft Forms?**

Per impostazione predefinita, Microsoft Forms è attivato per tutti gli utenti di un'organizzazione. Gli amministratori IT di Microsoft 365 possono disattivare Microsoft Forms nell'interfaccia di amministrazione di Microsoft 365, nella scheda ** Gestione utenti**. Per ulteriori informazioni, vedere [Configurare Microsoft Forms](set-up-microsoft-forms.md) e [Attivare o disattivare Microsoft Forms](turn-off-turn-on-microsoft-forms.md).

**Come è possibile fornire l'accesso a Microsoft Forms solo a utenti specifici dell'organizzazione?**

Gli amministratori possono modificare le autorizzazioni di accesso per persone specifiche nell'organizzazione. Vedere [Impostazioni amministratore in Microsoft Forms](administrator-settings-microsoft-forms.md).

## <a name="data-storage"></a>Archiviazione dei dati

**Dove vengono archiviati i dati per Microsoft Forms?**

I dati di Microsoft Forms vengono archiviati nei server negli Stati Uniti, ad eccezione dei dati per i tenant europei. I dati per i tenant basati europei vengono archiviati nei server in Europa.

## <a name="user-activity"></a>Attività utente

**Come si visualizzano le attività eseguite in Microsoft Forms dagli utenti dell'organizzazione?**

È possibile esaminare le [attività di Microsoft Forms](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities) nel log di controllo del [Centro sicurezza Microsoft 365](https://security.microsoft.com/?rfr=OfficeScc). Altre informazioni sul[Controllo in Office 365 (per amministratori)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906).

## <a name="user-account-information"></a>Informazioni sull'account utente

**Come è possibile verificare se un account utente è stato "eliminato definitivamente"?**

1. Gli amministratori possono accedere a [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).

2. Incollare l'URL seguente nella casella di ricerca superiore:

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*e-mail utente*: indirizzo di posta elettronica del proprietario del modulo che ha lasciato l'organizzazione e/o il cui account è stato disabilitato.

3. Fare clic su **Esegui query**.

Se le informazioni sull'account che stai cercando vengono restituite nella query, significa che l'account è stato eliminato temporaneamente ed è entro il limite di 30 giorni. Un amministratore globale può trasferire i moduli di proprietà dell'account eliminato temporaneamente utilizzando il metodo di trasferimento come descritto in precedenza.

Se le informazioni sull'account che si sta cercando non vengono restituite nella query, significa che l'account esiste ancora nel tenant di Office 365 o è stato eliminato più di 30 giorni fa. Se l'account esiste o è disabilitato nel tenant Office 365, un amministratore globale può trasferire i moduli di proprietà dell'account. Se l'account è stato "eliminato definitivamente" dal tenant di Office 365, un amministratore globale non sarà in grado di trasferire i moduli di proprietà di tale account. Anche questi moduli non sono ripristinabili.

**Esiste un limite al numero di utenti e alla quantità di dati archiviati per gli account utente anche dopo che questi hanno lasciato l'organizzazione?**

Attualmente non esiste alcun limite per il numero di utenti per i quali vengono conservati i dati, purché il provisioning dei loro account sia compreso nel contratto di servizio online dell'organizzazione. Inoltre, non esiste alcun limite per la quantità di dati archiviati per gli account utente.

**Cosa succede ai dati di un modulo se la licenza di Microsoft Forms del proprietario è stata rimossa o l'utente è stato disabilitato o eliminato dal tenant (Azure AD)?**

Se la licenza del proprietario è stata rimossa o l'account del proprietario è disabilitato, la quantità di dati archiviati per l'account utente non viene cambiata.

Se un account utente è stato eliminato dal tenant (Azure AD), tutti i dati relativi all'account verranno eliminati 30 giorni dopo l'eliminazione dell'utente.

## <a name="form-ownership-transfer"></a>Trasferimento della proprietà del modulo

**Il proprietario originale di un modulo non è più nell'organizzazione. Come posso trasferire la proprietà del modulo?**

Per trasferire il modulo di una persona che ha lasciato l'organizzazione, è necessario soddisfare i seguenti requisiti:

  - L'utente che compie il trasferimento è l'amministratore globale dell'organizzazione e dispone di una licenza Forms valida.

  - Il dipendente di cui si desidera trasferire il modulo dispone di un account eliminato o disabilitato.

  - Il modulo viene trasferito entro 30 giorni dall'eliminazione di un account.

> [!Note]
> Non esiste alcuna limitazione di tempo per trasferire la proprietà di un modulo da un account disabilitato (e non eliminato).

1. Se vengono soddisfatti tutti i requisiti, è possibile trasferire la proprietà del modulo. Nella barra degli indirizzi del browser sostituire l'URL esistente con quanto segue:

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*e-mail utente*: indirizzo di posta elettronica del proprietario del modulo che ha lasciato l'organizzazione e/o il cui account è stato disabilitato.
   > Ad esempio, se il proprietario del modulo ("Jason Fabian") ha lasciato l'organizzazione ("Contoso"), la soluzione alternativa per l'URL sarà simile alla seguente: `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. Ora si ha accesso ai moduli dell'ex dipendente. Nel modulo che si desidera trasferire fare clic su **Altre azioni** > ![ Altre opzioni](./media/image2.png) > **Sposta.**

   >[!Note]
   >Se si sta tentando di trasferire la proprietà del modulo a un dipendente attualmente attivo all'interno dell'organizzazione, è possibile spostarlo in un gruppo a cui appartiene. Se non si è già membri di tale gruppo, è necessario parteciparvi per eseguire il trasferimento. Al termine del trasferimento della proprietà del modulo, è possibile scegliere di lasciare il gruppo.

**Perché viene visualizzato un messaggio di errore quando si tenta di trasferire la proprietà di un modulo?**

Se viene visualizzato un messaggio di errore, uno dei seguenti motivi potrebbe impedire il trasferimento della proprietà:

|Messaggio di errore|Spiegazione|
| --- | --- |
| ***Non è possibile accedere a questa pagina***<br/><br/>Il proprietario del modulo ha ancora un account attivo. | Il proprietario del modulo dispone ancora di una licenza e di un account Forms attivi. |
| ***Non è possibile accedere a questa pagina***<br/><br/>Assicurati di aver inserito l'indirizzo di posta elettronica correttamente e che l'account del proprietario dei moduli non sia stato eliminato più di 30 giorni fa. | L'indirizzo di posta elettronica non è stato digitato correttamente e/o l'account del proprietario dei moduli è stato eliminato più di 30 giorni fa. |
| ***Non è possibile accedere a questa pagina***<br/><br/>Assicurarsi di aver inserito correttamente l'indirizzo di posta elettronica e quindi riprovare. | L'indirizzo di posta elettronica non è stato inserito o contiene errori di ortografia. |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Utilizzo dei moduli in Outlook o PowerPoint

**Gli utenti dell'organizzazione non sono in grado di aggiungere un sondaggio a indirizzo di posta elettronica di Outlook. Come è possibile risolvere il problema?**

L'impostazione **Autenticazione moderna** di Outlook deve essere abilitata per garantire che gli utenti dell'organizzazione possano [creare un sondaggio in Outlook](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0).

1. Accedere [https://admin.microsoft.com](https://admin.microsoft.com/) con l'account aziendale o dell'istituto di istruzione.

2. Selezionare **Impostazioni** \> **Impostazioni dell'organizzazione**.

   >[!Note]
   > Se non viene visualizzata l'opzione **Impostazioni**, selezionare il pulsante ![Altre opzioni >](./media/image2.png)**Mostra tutto** nel riquadro di sinistra.

3.  Selezionare **Autenticazione moderna.**

4.  Selezionare l'opzione **Attiva autenticazione moderna per Outlook 2013 per Windows e versioni successive (scelta consigliata)**.

Ulteriori informazioni sull'autenticazione moderna [e a più fattori](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide) e su come configurarla e implementarla nell'organizzazione.

**Non si desidera distribuire componenti aggiuntivi di Office per l'intera organizzazione. Gli utenti dell'organizzazione possono ancora utilizzare il componente aggiuntivo Moduli per PowerPoint?**

Sì, è possibile utilizzare la [distribuzione centralizzata](/office/dev/add-ins/publish/centralized-deployment) per distribuire solo il componente aggiuntivo Moduli per PowerPoint.

1.  Accedere [https://admin.microsoft.com](https://admin.microsoft.com/) con l'account aziendale o dell'istituto di istruzione.

2.  Selezionare **Impostazioni** \> **Componenti aggiuntivi**.

    >[!Note]
    >Se non viene visualizzata l'opzione **Impostazioni**, selezionare il pulsante ![Altre opzioni >](./media/image2.png)**Mostra tutto** nel riquadro di sinistra.

3.  Nell'elenco **Componenti aggiuntivi**, selezionare **Moduli**.

4.  In **Assegna utenti** nel riquadro **Modifica moduli** selezionare **Tutti**.

5.  Seleziona **Salva**.


## <a name="forms-and-anti-phishing"></a>Microsoft Forms e anti-phishing

**Cosa è possibile fare per il phishing e per potenziali intenti dannosi nei moduli all'interno del tenant?**

In Microsoft Forms vengono abilitate le revisioni automatiche dei computer per rilevare in modo proattivo la raccolta dannosa di dati sensibili nei moduli e poter bloccare temporaneamente tali moduli per evitare la raccolta di risposte.

Ulteriori informazioni su [Microsoft Forms e la prevenzione proattiva del phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

Se si è un amministratore globale e/o di sicurezza, è possibile accedere all'interfaccia di amministrazione di Microsoft 365 su [admin.microsoft.com](https://admin.microsoft.com/) e accedere al [Centro messaggi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter). In questo caso, verrà visualizzato un riepilogo giornaliero di tutti i moduli bloccati. Per ogni modulo elencato, è possibile scegliere se sbloccarlo o confermare il tentativo di phishing. Ulteriori informazioni su come [esaminare e sbloccare moduli o utenti rilevati e bloccati per potenziali tentativi di phishing.](review-unblock-forms-users-detected-blocked-potential-phishing.md)
