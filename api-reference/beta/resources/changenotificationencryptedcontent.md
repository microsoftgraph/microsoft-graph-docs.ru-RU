---
title: тип ресурса changeNotificationEncryptedContent
description: Объект changeNotificationEncryptedContent представляет зашифрованные данные, присоединенные к уведомлению об изменении.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 193f5eb36f19de1b3fd44112bf6bc56b19746911
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468746"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>тип ресурса changeNotificationEncryptedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет зашифрованные данные, присоединенные к уведомлению об изменении.

Подробные сведения см. [в материале Настройка уведомлений об изменении, включаем в себя данные ресурсов (предварительный просмотр).](/graph/webhooks-with-resource-data.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| data | Строка | Зашифрованные данные с кодом Base64, которые создают полный ресурс, повторно задав его в качестве JSON. Данные шифруются с помощью набора `dataKey` `AES/CBC/PKCS5PADDING` шифров. |
| dataSignature | Строка | Хэш HMAC-SHA256 с кодом Base64 для целей проверки. |
| dataKey | Строка | Симметричный ключ с кодом Base64, созданный Microsoft Graph для шифрования значения данных и создания подписи данных. Этот ключ шифруется с общедоступным ключом сертификата, который был предоставлен во время подписки. Его необходимо расшифровать с помощью закрытого ключа сертификата, прежде чем его можно будет использовать для расшифровки данных или проверки подписи. Этот ключ шифруется следующим набором шифров: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | string | ID сертификата, используемого для шифрования `dataKey` . |
| encryptionCertificateThumbprint | Строка | Hexadecimal representation of the thumbprint of the certificate used to encrypt the `dataKey` . |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->

```json
{
  "data": "{encrypted data that produces a full resource}",
  "dataSignature": "<HMAC-SHA256 hash>",
  "dataKey": "{encrypted symmetric key from Microsoft Graph}",
  "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
  "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
}
```

<!-- uuid: 564a955a-4837-424d-b7b8-3c6c33d5176d
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedConent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


