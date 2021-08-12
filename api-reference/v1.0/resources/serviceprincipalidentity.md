---
title: тип ресурса servicePrincipalIdentity
description: Модели основного удостоверения службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f486efbbfefb9639551c4d7fa587d056aaf3211e5b53dd8d212b7171b59baac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202121"
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
