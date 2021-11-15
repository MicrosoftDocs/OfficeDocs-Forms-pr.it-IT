---
title: Attivare o disattivare Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Questo articolo spiega come gli amministratori di Microsoft 365 possono disattivare o attivare Microsoft Forms per l’intera organizzazione o per persone specifiche dell’organizzazione.
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951461"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Attivare o disattivare Microsoft Forms

Per impostazione predefinita, [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)è attivato per tutti gli utenti dell'organizzazione. Gli amministratori di [ ](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504), possono [ configurare Microsoft Forms ](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240) e disattivarlo o riattivarlo per l'intera organizzazione o solo per persone specifiche.

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>Disattivare Microsoft Forms per tutti gli utenti dell'organizzazione

1.  Accedere a [Microsoft Azure ](https://portal.azure.com/).

2.  Nel riquadro sinistro fare clic su **Azure Active Directory **.

3.  Fare clic su **Applicazioni aziendali **.

4.  Spostarsi sui servizi necessari, quindi ripetere i passaggi da 5 a 7 sia per il ** tipo di applicazione**\> ** CollabDBService** che per le** applicazioni Microsoft** \> **Microsoft Forms**.
    
      - Nel campo di ricerca nell'elenco a discesa **Tipo di applicazione** digitare **CollabDBService**. Selezionare **CollabDBService ** dall’elenco dei risultati della ricerca.
    
      - **Nell'elenco a discesa** Tipo di applicazione **selezionare ** Applicazioni Microsoft. Nel campo di ricerca dell'elenco a discesa **Tipo di applicazione** digitare **Microsoft Forms**, quindi selezionare ** Microsoft Forms** dall'elenco dei risultati della ricerca.

5.  In **Gestisci** fare clic su **Proprietà**.

6.  Per l'opzione, **Abilitato per l'accesso utenti?**, selezionare **No**.

7.  Fare clic su **Salva**.

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>Disattivare Microsoft Forms per persone specifiche dell'organizzazione

1.  Accedere a Microsoft 365 come amministratore globale con il proprio account aziendale o dell'istituto di istruzione. [Informazioni su come eseguire l'accesso](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4).

2.  Nell'interfaccia di amministrazione di Microsoft 365 fare clic su **Utenti** \> **Utenti attivi**.

3.  Selezionare la casella accanto al nome della persona alla quale disattivare Microsoft Forms.

4.  Sulla barra multifunzione fare clic su ** Gestisci licenze prodotto.**

5.  Nel modulo dell'account che si apre nella scheda **Licenze e app** espandere la sezione App e scorrere verso il basso fino all'opzione Microsoft Forms. 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Modulo Opzioni account nell'interfaccia di amministrazione di Microsoft 365":::

6.  Deselezionare la casella per disattivare Microsoft Forms. Per attivarlo, selezionare la casella di controllo.

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Attiva/disattiva Microsoft Forms":::

     > [!Note]
     > [Controllare l’elenco](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e) per verificare se si dispone di una licenza Office che includa Microsoft Forms. Se la licenza è presente nell’elenco, bisognerà deselezionare la casella di controllo Microsoft Forms per disattivare del tutto l'accesso utente.

7.  Nella parte inferiore dell’elenco**delle App** fare clic su **Salva modifiche**.

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>Microsoft Forms risulta attivo, ma gli utenti dell'organizzazione non possono ancora accedervi

Controllare la seguente impostazione in Microsoft Azure per verificare che Microsoft Forms sia abilitato:

1.  Accedere a [Microsoft Azure ](https://portal.azure.com/).

2.  Nel riquadro sinistro fare clic su **Azure Active Directory **.

3.  Fare clic su **Applicazioni aziendali **.

4.  Spostarsi sui servizi necessari, quindi ripetere i passaggi da 5 a 7 sia per il ** tipo di applicazione**\> ** CollabDBService** che per le** applicazioni Microsoft** \> **Microsoft Forms**.
    
      - Nel campo di ricerca nell'elenco a discesa**Tipo di applicazione** digitare **CollabDBService**. Selezionare **CollabDBService ** dall’elenco dei risultati della ricerca.
    
      - **Nell'elenco a discesa** Tipo di applicazione **selezionare ** Applicazioni Microsoft. Nel campo di ricerca dell'elenco a discesa **Tipo di applicazione** digitare **Microsoft Forms**, quindi selezionare ** Microsoft Forms** dall'elenco dei risultati della ricerca.

5.  In **Gestisci** fare clic su **Proprietà**.

6.  Per l'opzione **Abilitato per l’accesso utenti?** selezionare **Sì**.

7.  Fare clic su **Salva**.

    >[!Note]
    >I servizi di SharePoint devono essere abilitati anche per consentire agli utenti dell'organizzazione di accedere a Microsoft Forms.

## <a name="feedback-for-microsoft-forms"></a>Feedback per Microsoft Forms

L'opinione degli utenti è importante\! Per inviare commenti e suggerimenti su Microsoft Forms, spostarsi nell'angolo in alto a destra del modulo e selezionare **Altre impostazioni del modulo** ![pulsante Altre opzioni ](./media/image2.png)\>**Feedback**.

