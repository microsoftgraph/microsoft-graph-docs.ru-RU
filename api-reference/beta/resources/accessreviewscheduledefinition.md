---
title: тип ресурса accessReviewScheduleDefinition
description: Представляет обзор доступа или серию обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a2ef3d4ccaaef05140ebc71f48825262cf34f956
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816051"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет планирование просмотра доступа Azure [AD.](accessreviewsv2-overview.md) 

AccessReviewScheduleDefinition содержит список [объектов accessReviewInstance](accessreviewinstance.md) . Каждое повторение определения расписания создает экземпляр. Экземпляры также представляют каждый проверяемый уникальный ресурс. Если в определении расписания рассматриваются несколько ресурсов (в том числе несколько групп), каждый ресурс имеет уникальный экземпляр на каждое повторение. В случае разовой проверки на ресурс создается только один экземпляр.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinitions](../api/accessreviewset-list-definitions.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Списки всех accessReviewScheduleDefinition. Не включает связанные объекты accessReviewInstance в результаты. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите accessReviewScheduleDefinition с указанным **id**. Не включает связанные объекты accessReviewInstance в результаты. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание нового accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удалите accessReviewScheduleDefinition с указанным **id**. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств accessReviewScheduleDefinition с указанным **id**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызываемая пользователь является рецензентом в одном или более экземплярах.|

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| additionalNotificationRecipients   |[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) collection| Определяет список дополнительных пользователей или членов группы, которые будут уведомлены о ходе проверки доступа. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший этот обзор. Только для чтения. |
| createdDateTime  |DateTimeOffset  | Timestamp, когда была создана серия обзоров доступа. Поддерживает `$select`. Только для чтения. |
| descriptionForAdmins  |String  |  Описание, предоставленное создателями обзора, чтобы предоставить администраторам дополнительный контекст обзора. Поддерживает `$select`. |
| descriptionForReviewers |Строка | Описание, предоставленное создателями обзора, чтобы предоставить рецензентам дополнительный контекст обзора. Рецензенты увидят это описание в отправленной им электронной почте с запросом на отзыв. Уведомления электронной почты поддерживают до 256 символов. Поддерживает `$select`. |
| displayName | Строка   | Имя серии обзоров доступа. Поддерживает `$select` и `$orderBy`. Требуется при создании. |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. См [. accessReviewReviewerScope](accessreviewreviewerscope.md). Заменяет **backupReviewers**. Поддерживает `$select`. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства будет проигнорировано, если в свойстве **stageSettings** будут назначены анализаторы откатов. |
| id | String | Уникальный идентификатор обзора доступа, назначенного функцией. Поддерживает `$select`. Только для чтения.|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Это свойство необходимо при проверке доступа гостевых пользователей ко всем группам Microsoft 365 и определяет, какие Microsoft 365 проверяются. Каждая группа станет уникальным **accessReviewInstance** из серии обзоров доступа.  Для поддерживаемых областей см [. accessReviewScope](accessreviewscope.md). Поддерживает `$select`. Примеры вариантов настройки instanceEnumerationScope см. в примере Настройка области определения обзора доступа с помощью [API Microsoft Graph.](/graph/accessreviews-scope-concept) |
| instances |[accessReviewInstance](../resources/accessreviewinstance.md) collection|  Набор экземпляров обзоров доступа для этой серии обзоров доступа. Обзоры доступа, которые не повторялись, будут иметь только один экземпляр; в противном случае для каждого повторения имеется экземпляр. |
| lastModifiedDateTime | DateTimeOffset   | Timestamp, когда в последний раз была изменена серия обзоров доступа. Поддерживает `$select`. Только для чтения.|
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения тех, кто является рецензентами. Свойство рецензентов может быть updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов. Требуется при создании. Поддерживает `$select`. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept) <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства будет игнорироваться, если рецензенты назначены через **свойство stageSettings** .  |
| область  |[accessReviewScope](../resources/accessreviewscope.md)  | Определяет объекты, доступ к которым просматривается. Для поддерживаемых областей см [. accessReviewScope](accessreviewscope.md). Требуется при создании. Поддерживает и `$select` `$filter` (`contains` только). Примеры параметров настройки области см. в примере Настройка области определения обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept) |
|stageSettings|[accessReviewStageSettings](../resources/accessreviewstagesettings.md) collection| Требуется только многоступенчатый обзор доступа для определения этапов и их параметров. Каждый экземпляр обзора можно разбить на три последовательного этапа, где на каждом этапе может быть разный набор рецензентов, рецензентов и параметров. Этапы будут создаваться последовательно на основе **свойства dependsOn** . Необязательное свойство.  <br/><br/>Когда это свойство определено, вместо соответствующих параметров в [объекте accessReviewScheduleDefinition](accessreviewscheduledefinition.md) используются его параметры **, рецензенты** и свойства **fallbackReviewers**. |
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для серии обзоров доступа см. ниже определение типа. Поддерживает `$select`. Требуется при создании. |
| status  |String   | Это поле только для чтения указывает состояние обзора доступа. Типичные состояния включают `Initializing`, `NotStarted``Starting`, , `InProgress`, `Completing`, , `Completed`и `AutoReviewing``AutoReviewed`.  <br>`$select`Поддерживает и `$orderby``$filter` (`eq`только). Только для чтения. |
| backupReviewers (обесценив) |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует.  Поддерживает `$select`. <br>**Примечание:** Это свойство было заменено **на fallbackReviewers**. Однако указание резервных **копийReviewers** или **fallbackReviewers** автоматически заполняет те же значения для другого свойства. |


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) collection         | Если это `accessReviewScheduleDefinition` повторяющийся обзор доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждый уникальный ресурс, рассмотренный в .`accessReviewScheduleDefinition` Если обзор имеет несколько ресурсов и несколько экземпляров, каждый ресурс будет иметь уникальный экземпляр для каждого повторения. |

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
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "backupReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "stageSettings": [
    {
      "@odata.type": "microsoft.graph.accessReviewStageSettings"
    }
  ],
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  },
  "additionalNotificationRecipients": [
    {
        "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem"
    }
  ]
}
```
