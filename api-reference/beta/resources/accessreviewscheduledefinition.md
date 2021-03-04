---
title: тип ресурса accessReviewScheduleDefinition
description: Представляет обзор доступа или серию обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e4820cf85d3160c04372df79072b4b40708ef868
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443182"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет планирование просмотра доступа Azure [AD.](accessreviewsv2-root.md) 

AccessReviewScheduleDefinition содержит список [объектов accessReviewInstance.](accessreviewinstance.md) Каждое повторение определения расписания создаст экземпляр. Экземпляры также представляют каждую уникальную группу, проверяемую. Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения. В случае разовой проверки будет создан только один экземпляр для одной группы.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Списки всех accessReviewScheduleDefinition. Не включает связанные экземпляры accessReviewInstance в списки. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите accessReviewScheduleDefinition с указанным id. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание нового accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удалите accessReviewScheduleDefinition с указанным идентификатором. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств accessReviewScheduleDefinition с указанным идентификатором. |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| id | String | Уникальный идентификатор обзора доступа, назначенного функцией.|
| displayName | String   | Имя серии обзоров доступа. Требуется при создании. |
| createdDateTime  |DateTimeOffset  | DateTime, когда была создана серия обзоров. |
| lastModifiedDateTime | DateTimeOffset   | DateTime при последней модификации серии обзоров.|
| status  |string   | Это поле только для чтения указывает состояние accessReview. Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| descriptionForAdmins  |string  |  Описание, предоставленное создателями обзора, чтобы предоставить администраторам дополнительный контекст обзора. |
| descriptionForReviewers |string | Описание, предоставленное создателями обзора, чтобы предоставить рецензентам дополнительный контекст обзора. Рецензенты увидят это описание в отправленной им электронной почте с запросом на отзыв. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший этот обзор. |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  | Определяет область рассмотренных пользователей. Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) Требуется при создании. |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | В случае проверки гостевых пользователей во всех группах Microsoft 365 это определяет область просмотра групп. Каждая группа станет уникальным accessReviewInstance из серии обзоров доступа.  Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) | 
| параметры  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для серии обзоров доступа см. ниже определение типа. |
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения тех, кто является рецензентами. См. [accessReviewReviewerScope.](accessreviewreviewerscope.md) Требуется при создании. |
| backupReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. См. [accessReviewReviewerScope.](accessreviewreviewerscope.md) |
| instances |Collection(microsoft.graph.accessReviewInstance)|  Набор экземпляров обзоров доступа для этой серии обзоров доступа. Обзоры доступа, которые не повторялись, будут иметь только один экземпляр; в противном случае для каждого повторения будет иметься экземпляр. |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) collection         | Если это `accessReviewScheduleDefinition` повторяющийся обзор доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждый уникальный ресурс, рассмотренный в `accessReviewScheduleDefinition` . Если обзор имеет несколько ресурсов и несколько экземпляров, каждый ресурс будет иметь уникальный экземпляр для каждого повторения. |

### <a name="supported-queries-for-accessreviewscheduledefinition"></a>Поддерживаемые запросы для accessReviewScheduleDefinition
Ниже приводится запросы, поддерживаемые [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md) на основе [accessReviewScope.](accessreviewscope.md)

|Сценарий| Запрос |
|--|--|
| Список всех отдельных групп (исключает определения для всех `accessReviewScheduleDefinition` групп Microsoft 365 с гостевых пользователей) | /beta/identityGovernance/accessReviews/definitions?$filter=contains (scope/query, '/groups') |
| Список каждого из них в определенной группе (исключает определения для всех `accessReviewScheduleDefinition` групп Microsoft 365 с гостевых пользователей) | /beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}') |
| Список всех `accessReviewScheduleDefinition` областей для всех групп Microsoft 365 с гостевых пользователей | /beta/identityGovernance/accessReviews/definitions?$filter=contains (scope/query, './members') |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
