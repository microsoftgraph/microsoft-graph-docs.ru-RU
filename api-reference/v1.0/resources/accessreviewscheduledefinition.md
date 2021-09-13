---
title: тип ресурса accessReviewScheduleDefinition
description: Представляет планирование просмотра доступа Azure AD.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23b13daba0ea86d2330bd8b6c7f59e27af967aec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084701"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

Представляет планирование просмотра доступа Azure [AD.](accessreviewsv2-root.md)

AccessReviewScheduleDefinition содержит список [объектов accessReviewInstance.](accessreviewinstance.md) Каждое повторение определения расписания создает экземпляр. Экземпляры также представляют каждый проверяемый уникальный ресурс. Если определение расписания проверяет несколько ресурсов, каждый ресурс имеет уникальный экземпляр на каждое повторение. В случае разовой проверки на ресурс создается только один экземпляр.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Списки всех accessReviewScheduleDefinition. Не включает связанные объекты accessReviewInstance в результаты. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите accessReviewScheduleDefinition с указанным **id**. Не включает связанные объекты accessReviewInstance в результаты. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание нового accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление accessReviewScheduleDefinition с указанным **id**. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств accessReviewScheduleDefinition с указанным **id**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызываемая пользователь является рецензентом в одном или более экземплярах.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| id | String | Уникальный идентификатор обзора доступа, назначенного функцией. Поддерживает `$select`. Только для чтения.|
| displayName | Строка   | Имя серии обзоров доступа. Поддерживает `$select` и `$orderBy`. Требуется при создании. |
| createdDateTime  |DateTimeOffset  | Timestamp, когда была создана серия обзоров доступа. Поддерживает `$select` и `$orderBy`. Только для чтения. |
| lastModifiedDateTime | DateTimeOffset   | Timestamp, когда в последний раз была изменена серия обзоров доступа. Поддерживает `$select`. Только для чтения.|
| status  |String   | Это поле только для чтения указывает состояние обзора доступа. Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  <br>Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения. |
| descriptionForAdmins  | Строка  |  Описание, предоставленное создателями обзора, чтобы предоставить администраторам дополнительный контекст обзора. Поддерживает `$select`. |
| descriptionForReviewers | Строка | Описание, предоставленное создателями обзора, чтобы предоставить рецензентам дополнительный контекст обзора. Рецензенты увидят это описание в отправленной им электронной почте с запросом на отзыв. Уведомления электронной почты поддерживают до 256 символов. Поддерживает `$select`. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший этот обзор. Только для чтения. |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  |  Определяет объекты, доступ к которым просматривается.  Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) Требуется при создании. Поддерживает `$select` и `$filter` `contains` (только). Примеры параметров настройки области см. в примере [Configure the scope of your access review definition using the Microsoft Graph API.](/graph/accessreviews-scope-concept) |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Это свойство необходимо при проверке доступа гостевых пользователей ко всем группам Microsoft 365 и определяет, какие Microsoft 365 проверяются. Каждая группа станет уникальным **accessReviewInstance** из серии обзоров доступа.  Для поддерживаемых областей [см. в поле accessReviewScope.](accessreviewscope.md) Поддерживает `$select`. Примеры вариантов настройки instanceEnumerationScope см. в примере Настройка области определения обзора доступа с помощью [API Microsoft Graph Microsoft.](/graph/accessreviews-scope-concept) | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для серии обзоров доступа см. ниже определение типа. Поддерживает `$select`. Требуется при создании. |
| рецензенты   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей обзора доступа используется для определения тех, кто является рецензентами. Свойство рецензентов может быть updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов. Требуется при создании. Поддерживает `$select`. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept) |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. См. [accessReviewReviewerScope.](accessreviewreviewerscope.md) Заменяет **backupReviewers**. Поддерживает `$select`. |

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
| instances|[accessReviewInstance](accessreviewinstance.md) collection | Если **accessReviewScheduleDefinition** является повторяемой проверкой доступа, экземпляры представляют каждое повторение. Обзор, который не повторяется, будет иметь точно один экземпляр. Экземпляры также представляют каждый уникальный ресурс, рассмотренный в **accessReviewScheduleDefinition.** Если обзор имеет несколько ресурсов и несколько экземпляров, каждый ресурс будет иметь уникальный экземпляр для каждого повторения. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "microsoft.graph.entity",
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
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
