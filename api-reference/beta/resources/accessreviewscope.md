---
title: Тип ресурса accessReviewScope
description: 'В функции проверки доступа Azure AD объекты, которые будут рассмотрены в `accessReviewScope` проверке доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133447"
---
# <a name="accessreviewscope-resource-type"></a>Тип ресурса accessReviewScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewScope** определяет, какие сущности будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это выражается как запрос odata. Тип запроса также должен быть выражен, чтобы сценарии можно было поддерживать для просмотра сущностями за пределами MicrosoftGraph, например ARM.

## <a name="properties"></a>Свойства
| Свойство   | Тип  | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос |Строка  | Запрос, определяющий, что будет рассмотрено. Примеры см. в таблице. |
|queryType  |Строка | Тип запроса. Примеры: MicrosoftGraph и ARM. |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>Поддерживаемые запросы для accessReviewScope в качестве области
Далее запросы поддерживаются в качестве `scope` свойства [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|-- |
| Проверка всех пользователей, которые назначены группе | /groups/{group id}/transitiveMembers ||
| Просмотр гостевых пользователей, присвоенных группе | /groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') ||
| Проверка гостевых пользователей, присвоенных всем группам | ./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') | Обратите внимание, что соответствующий экземплярEnumerationScope также следует передать в accessReviewScheduleDefinition. См. таблицу ниже для запроса instanceEnumerationScope. |
| Проверки пакета управления правами на доступ к данным | /identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')| Обратите внимание, что для проверки назначения пакета Access поддерживается только чтение|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>Поддерживаемые запросы для accessReviewScope как instanceEnumerationScope
Далее запросы поддерживаются в качестве `instanceEnumerationScope` свойства [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Сценарий| Запрос | Дополнительные комментарии |
|--|--|--|
| Просмотр гостевых пользователей, которые назначены всем группам, за исключением указанных групп | /groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true | Обратите внимание, что соответствующая область также должна быть передана в accessReviewScheduleDefinition. См. выше в таблице свойств области "Просмотр гостевых пользователей, присвоенных всем группам" запроса области. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
