---
title: тип ресурса printCertificateSigningRequest
description: Запрос на подписание сертификата (CSR), который будет использоваться при регистрации принтера в службе универсальной печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2136ae68a722242e8ad3b7f39743e20d7a54cfe7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944300"
---
# <a name="printcertificatesigningrequest-resource-type"></a>тип ресурса printCertificateSigningRequest

Пространство имен: microsoft.graph

Запрос на подписание сертификата (CSR), который будет использоваться при регистрации принтера в службе универсальной печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|content|String|Запрос сертификата pkcs10 с кодом base64. Только для чтения.|
|transportKey|String|Базовая часть асимметричного ключа, генерируемого клиентом. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printCertificateSigningRequest",
  "content": "String",
  "transportKey": "String"
}
```

