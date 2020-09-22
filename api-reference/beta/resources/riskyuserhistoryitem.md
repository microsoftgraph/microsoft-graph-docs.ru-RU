---
title: Тип ресурса Рискюсерхисторитем
description: Представляет историю риска для пользователей Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f91f07e889a1808696a0bfb7180b51aa06355334
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016172"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Тип ресурса Рискюсерхисторитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD. 

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Журнал списка](../api/riskyuser-list-history.md) | Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)|Получение журнала рисков пользователя Azure AD.|


## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| userId         | строка  | Идентификатор пользователя. |
| initiatedBy    | логический    | Идентификатор субъекта, который выполняет операцию. |
| activity       | [рискусерактивити](riskuseractivity.md)| Действие, связанное с изменением уровня риска пользователя. | 

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->


