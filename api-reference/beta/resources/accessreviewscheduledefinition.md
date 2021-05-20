---
title: тип ресурса accessReviewScheduleDefinition
description: Представляет обзор доступа или серию обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06556bfdbcad8c422e4e8e522163437c9c7fa9c6
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579909"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет планирование просмотра доступа Azure [AD.](accessreviewsv2-root.md) 

AccessReviewScheduleDefinition содержит список [объектов accessReviewInstance.](accessreviewinstance.md) Каждое повторение определения расписания создает экземпляр. Экземпляры также представляют каждый проверяемый уникальный ресурс. Если в определении расписания рассматриваются несколько ресурсов (в том числе несколько групп), каждый ресурс имеет уникальный экземпляр на каждое повторение. В случае разовой проверки на ресурс создается только один экземпляр.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Списки всех accessReviewScheduleDefinition. Не включает связанные объекты accessReviewInstance в результаты. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите accessReviewScheduleDefinition с указанным **id**. Не включает связанные объекты accessReviewInstance в результаты.|
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание нового accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление accessReviewScheduleDefinition с указанным **id**. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств accessReviewScheduleDefinition с указанным **id**. |

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| id | Строка | Уникальный идентификатор обзора доступа, назначенного функцией. Поддерживает `$select`.|
| displayName | Строка   | Имя серии обзоров доступа. Требуется при создании. Поддерживает `$select`. |
| createdDateTime  |DateTimeOffset  | Timestamp, когда была создана серия обзоров доступа. Поддерживает `$select`.|
| lastModifiedDateTime | DateTimeOffset   | Timestamp, когда в последний раз была изменена серия обзоров доступа. Поддерживает `$select`.|
| status  |String   | Это поле только для чтения указывает состояние обзора доступа. Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . <br>Поддерживает `$select` и `$orderby` `$filter` `eq` (только).|
| descriptionForAdmins  |строка  |  Описание, предоставленное создателями обзора, чтобы предоставить администраторам дополнительный контекст обзора. Поддерживает `$select`. |
| descriptionForReviewers |строка | Описание, предоставленное создателями обзора, чтобы предоставить рецензентам дополнительный контекст обзора. Рецензенты увидят это описание в отправленной им электронной почте с запросом на отзыв. Поддерживает `$select`. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший этот обзор. |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  | Определяет область ресурсов, которые необходимо просмотреть. Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) Требуется при создании. Поддерживает `$select` и `$filter` `contains` (только). Примеры параметров настройки области см. в примере [Configure the scope of your access review definition using the Microsoft Graph API.](/graph/accessreviews-scope-concept)|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Это свойство необходимо при проверке доступа гостевых пользователей ко всем группам Microsoft 365 и определяет, какие Microsoft 365 проверяются. Каждая группа станет уникальным **accessReviewInstance** из серии обзоров доступа.  Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) Поддерживает `$select`. Примеры вариантов настройки instanceEnumerationScope см. в примере Настройка области определения обзора доступа с помощью [API Microsoft Graph Microsoft.](/graph/accessreviews-scope-concept)| 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для серии обзоров доступа см. ниже определение типа. Поддерживает `$select`.|
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения тех, кто является рецензентами. Требуется при создании. Поддерживает `$select`. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept)|
| backupReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. Поддерживает `$select`. <br>**Примечание:** Это свойство было заменено **fallbackReviewers**. Однако указание резервных **копийReviewers** или **fallbackReviewers** автоматически заполняет те же значения для другого свойства.|
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. Поддерживает `$select`.|
| instances |[accessReviewInstance](../resources/accessreviewinstance.md) collection|  Набор экземпляров обзоров доступа для этой серии обзоров доступа. Обзоры доступа, которые не повторялись, будут иметь только один экземпляр; в противном случае для каждого повторения имеется экземпляр. |

## <a name="relationships"></a>Отношения

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) collection         | Если это `accessReviewScheduleDefinition` повторяющийся обзор доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждый уникальный ресурс, рассмотренный в `accessReviewScheduleDefinition` . Если обзор имеет несколько ресурсов и несколько экземпляров, каждый ресурс будет иметь уникальный экземпляр для каждого повторения. |

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
