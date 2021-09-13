---
title: тип ресурса servicePrincipalIdentity
description: Модели основного удостоверения службы.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae9d82ce65b7a6e8c82e0377df89939b9219f3db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108830"
---
# <a name="serviceprincipalidentity-resource-type"></a>тип ресурса servicePrincipalIdentity

Пространство имен: microsoft.graph

Модели основного удостоверения службы.

Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appId|String|Идентификатор приложения для директора службы.|
|displayName|String|Отображение имени основного удостоверения службы. Унаследованный от [удостоверения](../resources/identity.md)|
|id|Строка|Идентификатор основного удостоверения службы. Унаследованный от [удостоверения](../resources/identity.md)|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
