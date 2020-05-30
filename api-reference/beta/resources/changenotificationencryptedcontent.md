---
title: Тип ресурса Чанженотификатионенкриптедконтент
description: Подписка с данными ресурсов позволяет клиентскому приложению получать уведомления об изменениях, внесенные в данные в Microsoft Graph. Зашифрованное содержимое уведомления об изменении представляет зашифрованные данные, связанные с уведомлением.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1b89fcf99ed4a724bb86413d6ef369b121e28cd3
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430609"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>Тип ресурса Чанженотификатионенкриптедконтент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет зашифрованные данные, вложенные в уведомление об изменении.

Дополнительные сведения см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов (Предварительная версия)](/graph/webhooks-with-resource-data.md).

## <a name="methods"></a>Методы

Отсутствуют.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| data | string | Зашифрованные данные в кодировке Base64, которые создают полный респресентед ресурсов как JSON. Данные зашифрованы с `dataKey` помощью `AES/CBC/PKCS5PADDING` комплекта шифров. |
| Подпись | string | Хэш-код HMAC-SHA256 данных для целей проверки в кодировке Base64. |
| датакэй | string | Симметричный ключ в кодировке Base64, созданный Microsoft Graph для шифрования значения данных и создания подписи данных. Этот ключ шифруется с помощью открытого ключа сертификата, предоставленного во время подписки. Его необходимо расшифровать с помощью закрытого ключа сертификата, прежде чем его можно будет использовать для расшифровки данных или проверки подписи. Этот ключ зашифрован с помощью следующего комплекта шифра: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| енкриптионцертификатеид | string | Идентификатор сертификата, используемого для шифрования `dataKey` . |
| енкриптионцертификатесумбпринт | string | Шестнадцатеричное представление отпечатка сертификата, используемого для шифрования `dataKey` . |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
