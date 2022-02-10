---
title: тип ресурса riskyServicePrincipalHistoryItem
description: Представляет историю рисков для директоров служб Azure AD
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aaafd1236a31530c32ca9cb6f62db932a0588f9e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519983"
---
# <a name="riskyserviceprincipalhistoryitem-resource-type"></a>тип ресурса riskyServicePrincipalHistoryItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Представляет историю рисков для директора службы Azure AD, определяемую службой Azure AD Identity Protection. Наследует от [riskyServicePrincipal](riskyserviceprincipal.md).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[История списка](../api/riskyserviceprincipal-list-history.md) | [коллекция riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md)|Получите историю рисков для директора службы Azure AD.|


## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| servicePrincipalId         | string  | Идентификатор директора службы. |
| initiatedBy    | логический    | Идентификатор субъекта операции. |
| действие       | [riskServicePrincipalActivity](riskserviceprincipalactivity.md)| Действие, связанное с изменением уровня основного риска службы. | 

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyServicePrincipalHistoryItem",
  "baseType": "microsoft.graph.riskyServicePrincipal"
}-->

```json
{
    "servicePrincipalId": "String",
    "initiatedBy": "String",
    "activity": {"@odata.type": "microsoft.graph.riskServicePrincipalActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyServicePrincipalHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
