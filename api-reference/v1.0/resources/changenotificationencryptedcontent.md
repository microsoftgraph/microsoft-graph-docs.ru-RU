---
title: тип ресурса changeNotificationEncryptedContent
description: Объект changeNotificationEncryptedContent представляет зашифрованные данные, присоединенные к уведомлению об изменении.
ms.localizationpriority: medium
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 3ca826bd2790fef77dd78f183a34fc306f28e47b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126949"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>тип ресурса changeNotificationEncryptedContent

Пространство имен: microsoft.graph

Представляет зашифрованные данные, присоединенные к уведомлению об изменении.

Дополнительные сведения см. в выпуске Настройка уведомлений об изменении, которые [включают данные ресурсов (предварительный просмотр).](/graph/webhooks-with-resource-data.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| data | string | Зашифрованные данные с кодом Base64, которые создают полный ресурс, повторно задав его в качестве JSON. Данные шифруются с помощью набора `dataKey` `AES/CBC/PKCS5PADDING` шифров. |
| dataSignature | string | Хэш HMAC-SHA256 с кодом Base64 для целей проверки. |
| dataKey | string | Симметричный ключ с кодом Base64, созданный корпорацией Майкрософт Graph для шифрования значения данных и создания подписи данных. Этот ключ шифруется с общедоступным ключом сертификата, который был предоставлен во время подписки. Его необходимо расшифровать с помощью закрытого ключа сертификата, прежде чем его можно будет использовать для расшифровки данных или проверки подписи. Этот ключ шифруется следующим набором шифров: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | string | ID сертификата, используемого для шифрования `dataKey` . |
| encryptionCertificateThumbprint | string | Hexadecimal representation of the thumbprint of the certificate used to encrypt the `dataKey` . |

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

<!-- uuid: 6bb14c3d-16ef-4ea3-8dc7-c88b9190081c
2020-08-05 14:57:30 UTC -->
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
