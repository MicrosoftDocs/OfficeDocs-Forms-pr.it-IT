---
title: Configurare Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Informazioni su come gli amministratori di Microsoft 365 possono controllare il modo in cui viene usato Microsoft Forms all'interno dell’organizzazione. Vengono inoltre fornite le risposte alle domande sulla sicurezza e sulla conformità, ad esempio, dove vengono archiviati i dati di Microsoft Forms.
ms.openlocfilehash: abee1557f379f646b277866f32fc0640c0b643cd
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951467"
---
# <a name="set-up-microsoft-forms"></a>Configurare Microsoft Forms


## <a name="overview"></a>[Panoramica](#tab/overview)

Microsoft Forms consente agli utenti di creare quiz, sondaggi, questionari, registrazioni e molto altro ancora, in modo facile e veloce. Quando si crea un quiz o un modulo, è possibile invitare gli altri a rispondere mediante un browser Web browser, perfino su dispositivi mobili. Una volta inviati i risultati, è possibile utilizzare l'analisi predefinita per valutare le risposte. I dati dei moduli, come i risultati di quiz, possono essere esportati facilmente su Excel per un'ulteriore analisi o classificazione.

Per ulteriori informazioni, vedere [Che cos'è Microsoft Forms?](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) In alternativa, vedere [ il post di blog di Microsoft 365](https://go.microsoft.com/fwlink/?linkid=852256)su Microsoft Forms.

>[!Note]
>Microsoft Forms è generalmente disponibile per i clienti di Office 365 Education, Microsoft 365 Apps for business e per i clienti con account Microsoft (Hotmail, Live o Outlook.com).

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="Anteprima dell'aspetto di un modulo su un dispositivo mobile.":::

## <a name="configure"></a>[Configurare](#tab/configure)

Gli amministratori di Microsoft 365 possono controllare le modalità di utilizzo di Microsoft Forms all’interno dell'organizzazione attraverso le seguenti attività:

<table>
<thead>
<tr class="header">
<th><strong>Attività di amministrazione</strong></th>
<th><strong>Descrizione</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Attivare o disattivare Microsoft Forms</strong></td>
<td>Microsoft Forms è attivato per impostazione predefinita per l’intera organizzazione. È sempre possibile <a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">disattivarlo</a> in qualsiasi momento.</td>
</tr>
<tr class="even">
<td><strong>Disattivare Microsoft Forms per specifiche persone dell'organizzazione</strong></td>
<td>Quando Microsoft Forms viene disattivato per una persona specifica, quest’ultima non potrà usarlo e il riquadro <strong>Forms</strong> non verrà più visualizzato nell'icona di avvio delle app o nella home page di Microsoft 365.  Informazioni su come <a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">disattivare i moduli per persone specifiche</a>. </td>
</tr>
<tr class="odd">
<td><strong>Configurare l'accesso condizionale di Azure Active Directory per Microsoft Forms</strong></td>
<td><p>Per configurare i criteri di accesso condizionale per Microsoft Forms, consultare la <a href="/azure/active-directory/conditional-access/"> documentazione sull’accesso condizionale di Azure AD</a> e includere <strong>Microsoft Form</strong> nelle assegnazioni delle <strong>app cloud</strong>.</p>
<p><strong>Nota:</strong> Se gli utenti dell'organizzazione risultano ancora bloccati dopo aver configurato l'accesso condizionale per Microsoft Forms, verificare che sia stato concesso l'accesso, tramite accesso condizionale, anche a SharePoint Online e a Exchange Online. <a href="/azure/active-directory/conditional-access/conditional-access-for-exo-and-spo">Altre informazioni</a>.</p></td>
</tr>
<tr class="even">
<td><strong>Controllare le impostazioni di condivisione esterna, registrare i nomi delle persone nell'organizzazione e/o proteggere i moduli dal phishing</strong></td>
<td><p>Nell’interfaccia di amministrazione di Microsoft 365 è possibile:</p>
<ul>
<li><p>Controllare che gli utenti esterni siano o meno autorizzati a collaborare a un modulo o a un quiz, con gli utenti dell'organizzazione.</p></li>
<li><p>Scegliere se acquisire o meno i nomi delle persone dell'organizzazione che compilano i moduli.</p></li>
<li><p>Disattivare o attivare il rilevamento automatico di phishing nei moduli.</p></li>
</ul>
<p>Altre informazioni sulle <a href="https://support.microsoft.com/office/administrator-settings-for-microsoft-forms-48161c55-fbae-4f37-8951-9e3befc0248b">impostazioni di amministrazione</a>.</p></td>
</tr>
<tr class="odd">
<td><strong>Consentire agli utenti di inserire un modulo PowerPoint</strong></td>
<td><ol type="1">
<li><p>Accedere a <a href="https://admin.microsoft.com/">https://admin.microsoft.com</a>.</p></li>
<li><p>Fare clic su <strong>Impostazioni</strong> &gt; <strong>Impostazioni</strong>.</p></li>
<li><p>Nella scheda <strong>Servizi</strong> della pagina <strong>Impostazioni</strong> fare clic su <strong>App e servizi di proprietà dell'utente</strong>.</p></li>
<li><p>Selezionare l'opzione <strong> Consenti agli utenti di accedere a Office store</strong>, per permettere agli utenti di inserire un modulo in PowerPoint.</p></li>
</ol>
<blockquote>
<p>Tenere presente che, l'applicazione della modifica potrebbe richiedere alcune ore. <a href="/office365/admin/manage/manage-deployment-of-add-ins>Learn more</a>.</p>
</blockquote></td>
</tr>
</tbody>
</table>


## <a name="security--compliance"></a>[Sicurezza e conformità](#tab/security)

Questo articolo si rivolge alle organizzazioni che devono rispettare determinati standard legali, normativi e tecnici per la sicurezza dei contenuti e l'utilizzo dei dati.

**Dove vengono archiviati i dati di Microsoft Forms?**

I dati di Microsoft Forms vengono archiviati in server situati negli Stati Uniti e in Europa. Tutti i dati sono conservati negli Stati Uniti, eccetto i tenant basati in Europa che hanno iniziato a usare Microsoft Forms dopo il maggio 2017. I dati vengono archiviati in database situati in Europa.

**Microsoft Forms è conforme?**

Microsoft Forms soddisfa i requisiti di conformità del GDPR dal maggio 2018. Per altre informazioni, vedere [ Microsoft 365 Richieste degli interessati per il GDPR](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json).

**Le protezioni FERPA e BAA sono applicate?**

Microsoft Forms soddisfa gli standard di protezione [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) e [BAA](https://www.microsoft.com/TrustCenter/Compliance/HIPAA).

*Esiste un limite al numero di utenti e alla quantità di dati archiviati per gli account utente anche dopo che questi hanno lasciato l'organizzazione?*

Attualmente non esiste alcun limite per il numero di utenti per i quali vengono conservati i dati, purché il provisioning dei loro account sia compreso nel contratto di servizio online dell'organizzazione. Inoltre, non esiste alcun limite per la quantità di dati archiviati per gli account utente.

*Il proprietario originale di un modulo non è più nell’organizzazione e/o la licenza Microsoft Forms è stata rimossa. Cosa succede ai dati associati al modulo precedentemente creato?*

Tutti i dati relativi all'account verranno eliminati 30 giorni dopo l'eliminazione dell’account utente dal tenant (Azure AD).

## <a name="faq"></a>Domande frequenti

**A quali usi si presta Microsoft Forms?**

Microsoft Forms è un'app semplice e leggera che consente di creare facilmente quiz, questionari e sondaggi. Negli istituti di istruzione può essere usato per creare test, raccogliere i feedback di insegnanti e genitori o pianificare le attività di classe e del personale. Nelle organizzazioni aziendali può essere usato per raccogliere i feedback dei clienti, misurare la soddisfazione dei dipendenti, migliorare i prodotti o il lavoro oppure organizzare eventi aziendali.

**Chi può usare Microsoft Forms?**

Microsoft Forms è gratuito per chiunque abbia un account Microsoft (Hotmail, Live o Outlook.com). Anche i seguenti clienti di Office 365 Education e Microsoft 365 Apps for business possono usare Microsoft Forms:

Office 365 Education

  - Office 365 A1 Plus

  - Office 365 A5

  - Clienti attuali che hanno acquistato Office 365 Education E3 prima del ritiro

Microsoft 365 Apps for business

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - Microsoft 365 Apps for enterprise

  - Piani di Microsoft 365 Enterprise E1, E3 ed E5

  - Clienti attuali di Office 365 Enterprise E4 che hanno acquistato E4 prima del ritiro

Accedere a [forms.office.com](https://forms.office.com/) e iniziare a creare sondaggi, quiz e test.

**Anche gli utenti sprovvisti di account Microsoft 365 possono inviare un sondaggio o un quiz su Microsoft Forms?**

Gli autori di Microsoft Forms possono attivare o disattivare le impostazioni per consentire agli utenti esterni all’organizzazione di rispondere a sondaggi o quiz. In questo caso, le risposte verranno inviate in modalità anonima. Per verificare chi ha compilato il sondaggio o il quiz, si può chiedere ai partecipanti di inserire il proprio nome nel questionario.

**Qual è il limite di numero di moduli che è possibile creare e il numero di risposte che un modulo può ricevere?**

I clienti di Office 365 Education e Microsoft 365 Apps for business possono creare fino a 200 moduli e ciascun modulo può ricevere fino a 50.000 risposte. Gli utenti di Microsoft Forms con account Microsoft (Hotmail, Live o Outlook.com) possono creare fino a 200 moduli e ciascun modulo può ricevere fino a 1.000 risposte per gli account a pagamento e fino a 200 risposte per gli account gratuiti. Altre informazioni sui limiti di [moduli, domande, risposte e caratteri in Forms.](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea)

Per avere a disposizione più risposte, è consigliabile esportare quelle esistenti in una cartella di lavoro di Excel e poi eliminarle dal sondaggio o dal quiz. Una volta eliminate, sarà possibile raccogliere più risposte.

**Con quali Web browser è compatibile Microsoft Forms?**

Microsoft Forms è ottimizzato per Internet Explorer 11, Edge, Chrome (ultima versione), Firefox (ultima versione), Chrome su Android (ultima versione) e Safari su iOS (ultima versione).

**In quali lingue è disponibile Microsoft Forms?**

Vedere [lingue supportate](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) e [ impostazioni lingua](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27) di Microsoft Forms.

**Microsoft Forms sostituirà Microsoft InfoPath?**

No. Microsoft InfoPath era una soluzione per creare moduli personalizzabili in grado di abilitare flussi di lavoro automatizzati, mentre Microsoft Forms è un'app semplice e leggera per la raccolta rapida di informazioni tramite sondaggi e quiz.

Microsoft InfoPath è stato sostituito da Elenchi SharePoint, Flusso e PowerApps, soluzioni moderne per la digitalizzazione del moduli aziendali tradizionali, l'automazione dei flussi di lavoro e la trasformazione dei processi di business. [Altre informazioni](https://products.office.com/business/business-process-automation).

**Come si fa a inviare feedback, per segnalare, ad esempio, bug di un prodotto o richiedere caratteristiche?**

L'opinione degli utenti è importante\! Per inviare commenti e suggerimenti su Microsoft Forms, spostarsi nell'angolo in alto a destra del modulo e selezionare **Altre impostazioni del modulo** ![pulsante Altre opzioni ](./media/image2.png)\>**Feedback**.

>[!Note]
>Per altre informazioni, vedere [Domande frequenti su Microsoft Forms](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c).

