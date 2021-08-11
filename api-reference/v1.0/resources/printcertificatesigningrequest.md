---
title: тип ресурса printCertificateSigningRequest
description: Запрос на подписание сертификата (CSR), который будет использоваться при регистрации принтера в службе универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0c86e7a2ecbd164f40dcbb0865954c4549622f16aa1f2b008a392f150b626aa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129984"
---
# <a name="printcertificatesigningrequest-resource-type"></a>тип ресурса printCertificateSigningRequest

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

