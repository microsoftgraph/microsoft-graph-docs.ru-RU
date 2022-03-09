---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b9f29b24c419c84fe8d7ff4b103a016e233d5746
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
    templateId: '62375ab9-6b52-47ed-826b-58e47e0e304b',
    values: [
        {
            name: 'GuestUsageGuidelinesUrl',
            value: 'https://privacy.contoso.com/privacystatement'
        },
        {
            name: 'EnableMSStandardBlockedWords',
            value: 'true'
        },
        {
            name: 'EnableMIPLabels',
            value: 'true'
        },
        {
            name: 'PrefixSuffixNamingRequirement',
            value: '[Contoso-][GroupName]'
        }
    ]
};

await client.api('/settings')
    .version('beta')
    .post(directorySetting);

```