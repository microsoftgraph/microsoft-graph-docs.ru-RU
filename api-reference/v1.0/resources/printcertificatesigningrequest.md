---
title: тип ресурса printCertificateSigningRequest
description: Запрос на подписание сертификата (CSR), который будет использоваться при регистрации принтера в службе универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4c3eda94bb0809991fe7f711a5290561ef1821d7
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517953"
---
# <a name="printcertificatesigningrequest-resource-type"></a>тип ресурса printCertificateSigningRequest

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Запрос на подписание сертификата (CSR), который будет использоваться при регистрации принтера в службе универсальной печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|content|String|Запрос сертификата pkcs10 с кодом base64. Только для чтения.|
|transportKey|Строка|Базовая часть асимметричного ключа, генерируемого клиентом. Только для чтения.|

## <a name="relationships"></a>Отношения
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

