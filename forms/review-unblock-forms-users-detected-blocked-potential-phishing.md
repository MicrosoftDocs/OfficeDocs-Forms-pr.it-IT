---
title: Esaminare e sbloccare i moduli o gli utenti individuati e bloccati per potenziale phishing
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms consente di eseguire revisioni automatiche dei computer per rilevare in modo proattivo, raccolte dati sensibili dannose in moduli e sondaggi. Gli amministratori globali e/o della sicurezza possono accedere all’interfaccia di amministrazione di Microsoft 365 per rivedere e sbloccare i moduli rilevati e bloccati a causa di potenziali tentativi di phishing e intenti dolosi.
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951498"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>Esaminare e sbloccare i moduli o gli utenti individuati e bloccati per potenziale phishing

In Microsoft Forms vengono abilitate le revisioni automatiche dei computer per rilevare in modo proattivo la raccolta dannosa di dati sensibili nei moduli e bloccare temporaneamente tali moduli per evitare la raccolta di risposte. Ulteriori informazioni su [Microsoft Forms e la prevenzione proattiva del phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

>[!Note]
>I passaggi descritti in questo documento si applicano anche a [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p?linkid=2128500) (in precedenza noto come Forms Pro). Si noti che è necessario disporre di una licenza di Dynamics 365 Customer Voice per sbloccare i sondaggi di Dynamics 365 Customer Voice. [Altre informazioni](/dynamics365/customer-voice/help-hub).

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>Esaminare gli avvisi nel portale di Microsoft 365 Defender

Gli amministratori globali o della sicurezza, riceveranno avvisi nel portale[Microsoft 365 Defender](https://security.microsoft.com/) riguardo i potenziali moduli di phishing per i quali è possibile intervenire.

>[!Note]
> Gli amministratori globali, riceveranno messaggi sulla privacy dei dati dell'organizzazione, incluse le notifiche giornaliere di qualsiasi modulo creato all'interno del tenant rilevato e bloccato per potenziali tentativi di phishing. Queste notifiche verranno visualizzate nel [Centro messaggi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) cercando le **notifiche di phishing di Microsoft Forms**. (Se non si visualizza questa notifica nella scheda/visualizzazione **Tutti i messaggi attivi** è possibile trovarla nella scheda/visualizzazione **Messaggi ignorati**). Per ciascuna notifica, selezionare il collegamento o i collegamenti URL di **revisione dell'amministratore di moduli ** per esaminare i moduli bloccati.  
  
Per consentire agli amministratori della sicurezza di ricevere notifiche anche su potenziali moduli di phishing, gli amministratori globali dovranno assegnare loro il ruolo con [autorizzazioni di lettura della privacy per il Centro messaggi](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader). Per ulteriori informazioni sul Centro messaggi, vedere le [domande frequenti](/microsoft-365/admin/manage/message-center). Vedere anche [come impostare le preferenze di posta elettronica per i messaggi di privacy dei dati](/microsoft-365/admin/manage/message-center#preferences).

1.  Accedere al [portale di Microsoft 365 Defender](https://security.microsoft.com/).

2.  Selezionare **Incidenti e avvisi** \> **Avvisi**. È possibile che vengano visualizzati uno o tutti i seguenti avvisi per Forms:
    
      - **L'utente non può condividere moduli e raccogliere risposte**
    
      - **Modulo contrassegnato e confermato come phishing**
    
      - **Modulo bloccato a causa di un potenziale tentativo di phishing**

3.  Selezionare un avviso per esaminarlo. Per esaminare il modulo contrassegnato, toccare o fare clic sui tre puntini nell'angolo in basso a destra accanto al pulsante **Gestisci avviso,** quindi selezionare **Rivedi modulo**.
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="Opzione Rivedi modulo":::

    >[!Tip]
    >Altre informazioni su [criteri di avviso in Microsoft 365](/microsoft-365/compliance/alert-policies).

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>Sbloccare un modulo o confermare il tentativo di phishing

Per ogni modulo esaminato, è possibile scegliere se sbloccarlo o confermare il phishing.

### <a name="unblock"></a>Sblocca

Selezionare **Sblocca** se si ritiene che il modulo non abbia finalità dannose.

>[!Note]
>Se qualcuno nel tenant richiede di sbloccare un modulo, consigliamo di richiedere informazioni specifiche sul modulo (ad esempio, data e ora del blocco, titolo), in modo tale da identificare efficacemente la notifica nell'interfaccia di amministrazione. Dato che le notifiche vengono inviate su base giornaliera, includendo tutti i moduli rilevati nelle ultime 24 ore, le informazioni d'identificazione del modulo saranno di grande utilità.

### <a name="confirm-phishing"></a>Conferma phishing

Selezionare **Conferma phishing** se si ritiene che il modulo abbia finalità dannose. Il modulo verrà bloccato definitivamente e il proprietario non sarà più in grado di modificarlo o di eliminarlo.

Dopo aver selezionato **Conferma phishing,** toccare o fare clic su ** Elimina modulo** per eliminare definitivamente il modulo dal tenant. È consigliabile reimpostare immediatamente la password dell’account del tenant che si ritiene compromesso.

>[!Tip]
>La selezione di **Conferma phishing** consente a Microsoft Forms di migliorare l'accuratezza di dei rilevamenti. 

## <a name="commonly-asked-questions"></a>Domande frequenti

**Quando si passa alla revisione di un modulo bloccato, per quale motivo non sono disponibili le opzioni di sblocco o conferma del phishing?**

Dopo la revisione, potrebbe riscontrarsi che il blocco di un modulo fosse già stato rimosso. In questo caso, il proprietario del modulo ha rimosso le parole chiave contrassegnate per potenziali tentativi di phishing, nel lasso di tempo in cui il modulo bloccato veniva esaminato. In tale scenario non sono richieste ulteriori azioni da parte dell'utente.

**Se un modulo è stato bloccato perché confermato come phishing, è possibile rimuoverlo?**

Se il modulo è già stato bloccato perché confermato come phishing, selezionare **Elimina modulo** per rimuoverlo dal tenant.

**Cosa succede se non si esegue alcuna azione su un modulo bloccato?**

Se si sceglie di non eseguire alcuna azione (sbloccare un modulo o confermarne l'intento di phishing), il modulo resterà bloccato. Il proprietario del modulo può comunque modificarlo e rimuovere le parole chiave contrassegnate per il potenziale tentativo di phishing.

**E se si volesse modificare o eliminare il contenuto bloccato nel modulo?**

Se si preferisce modificare e/o eliminare il contenuto bloccato, è possibile generare una pagina di creazione condivisa e gestire il modulo come coautori. A tale scopo, fare clic sul collegamento ** apri una pagina di creazione condivisa** che si trova nella messaggistica sopra il modulo che si sta esaminando.

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>Rimuovere le restrizioni per gli utenti di Microsoft Forms bloccati

Microsoft Forms blocca gli utenti che hanno tentato ripetutamente di raccogliere informazioni personali o riservate dalla distribuzione dei moduli e dalla raccolta di risposte. Gli amministratori globali ricevono una notifica sugli utenti bloccati attraverso il [Centro messaggi.](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) Se si ritiene che l’utente bloccato non abbia intenti dannoso e il suo account sia sicuro, si potrà eseguire la seguente procedura per sbloccarlo.

>[!Note]
>Gli amministratori della sicurezza potranno anche ricevere delle notifiche sui potenziali moduli di phishing, una volta che l’amministratore globale gli avrà assegnato il ruolo di [lettore della privacy per il Centro messaggi](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader).

1.  Passare al [Centro messaggi ](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) e cercare la notifica **Impedisci/Correggi: Microsoft Forms ha rilevato potenziali phishing.**

    >[!Note]
    >Se non si visualizza la notifica nella scheda/visualizzazione ** Tutti i messaggi attivi** sarà possibile trovarla nella scheda/visualizzazione **Messaggi ignorati**.
 
    Questa notifica contiene l’elenco degli utenti nel tenant a cui viene impedito di condividere moduli e raccogliere risposte.

2.  Fare clic sul collegamento fornito nella notifica per esaminare gli utenti bloccati.

3.  Per ogni utente che si ritiene non abbia intenti dannosi, è possibile scegliere di fare clic sul collegamento **Sblocca** nella colonna **Azioni** associata all’utente.

    >[!Note]
    >Se si ritiene che l’utente abbia intenti dannosi, non sono richieste ulteriori azioni da parte dell'utente.

    >[!Note]
    >La rimozione delle restrizioni potrebbe richiedere almeno 30 minuti.

