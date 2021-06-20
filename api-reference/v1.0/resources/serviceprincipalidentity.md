---
title: тип ресурса servicePrincipalIdentity
description: Модели основного удостоверения службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 231a0d9dc811569de23412d6ad76a2ba35f6c58b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031369"
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
|id|String|Идентификатор основного удостоверения службы. Унаследованный от [удостоверения](../resources/identity.md)|

## <a name="relationships"></a>Связи
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
