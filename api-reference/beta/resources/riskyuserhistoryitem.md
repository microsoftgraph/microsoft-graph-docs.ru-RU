---
title: Тип ресурса riskyUserHistoryItem
description: Представляет журнал рисков для пользователей Azure AD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6a415325c26226ad2400ce572146bbfaa5beb8c7
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060670"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Тип ресурса riskyUserHistoryItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Представляет журнал рисков пользователя Azure AD, определенный защитой идентификации Azure AD.

>[!NOTE]
> 1. Для использования этого API требуется Azure AD Premium P2 лицензия.
> 2. Доступность данных журнала рисков регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Журнал списков](../api/riskyuser-list-history.md) | [Коллекция riskyUserHistoryItem](riskyuserhistoryitem.md)|Получение журнала рисков пользователя Azure AD.|


## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| userId         | строка  | Идентификатор пользователя. |
| initiatedBy    | логический    | Идентификатор субъекта, который выполняет операцию. |
| действие       | [riskUserActivity](riskuseractivity.md)| Действие, связанное с изменением уровня риска пользователя. | 

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


