---
title: тип ресурса changeNotificationEncryptedContent
description: Объект changeNotificationEncryptedContent представляет зашифрованные данные, присоединенные к уведомлению об изменении.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: eab67f8a390b6522f963b004670e31e256078353
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334109"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>тип ресурса changeNotificationEncryptedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет зашифрованные данные, присоединенные к уведомлению об изменении.

Подробные сведения см. [в материале Настройка уведомлений об изменениях, которые включают данные ресурсов (предварительный просмотр).](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| data | string | Зашифрованные данные с кодом Base64, которые создают полный ресурс, повторно задав его в качестве JSON. Данные шифруются с помощью `dataKey` `AES/CBC/PKCS5PADDING` набора шифров. |
| dataSignature | string | Хэш HMAC-SHA256 с кодом Base64 для целей проверки. |
| dataKey | Строка | Симметричный ключ с кодом Base64, созданный корпорацией Майкрософт Graph для шифрования значения данных и создания подписи данных. Этот ключ шифруется с общедоступным ключом сертификата, который был предоставлен во время подписки. Его необходимо расшифровать с помощью закрытого ключа сертификата, прежде чем его можно будет использовать для расшифровки данных или проверки подписи. Этот ключ шифруется следующим набором шифров: `RSA/ECB/OAEPWithSHA1AndMGF1Padding`. |
| encryptionCertificateId | string | ID сертификата, используемого для шифрования `dataKey`. |
| encryptionCertificateThumbprint | Строка | Hexadecimal representation of the thumbprint of the certificate used to encrypt the `dataKey`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationEncryptedContent",
  "data": "String",
  "dataSignature": "String",
  "dataKey": "String",
  "encryptionCertificateId": "String",
  "encryptionCertificateThumbprint": "String"
}
```

<!-- uuid: 564a955a-4837-424d-b7b8-3c6c33d5176d
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


