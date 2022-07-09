---
title: Тип ресурса accessReviewScheduleDefinition
description: Представляет серию проверки доступа или проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8df583c8b1993ed7603e1ed56bfbc88e8749bc65
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698089"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Тип ресурса accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет планирование проверки Azure AD [доступа](accessreviewsv2-overview.md). 

AccessReviewScheduleDefinition содержит список [объектов accessReviewInstance](accessreviewinstance.md) . Каждое повторение определения расписания создает экземпляр. Экземпляры также представляют каждый проверяемый уникальный ресурс. Если определение расписания проверяет несколько ресурсов (включая несколько групп), каждый ресурс имеет уникальный экземпляр для каждого повторения. В случае однофакторной проверки создается только один экземпляр для каждого ресурса.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов accessReviewScheduleDefinitions](../api/accessreviewset-list-definitions.md) | [Коллекция accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Выводит список всех элементов accessReviewScheduleDefinition. Не включает связанные объекты accessReviewInstance в результаты. |
|[Получение accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получение объекта accessReviewScheduleDefinition с указанным **идентификатором**. Не включает связанные объекты accessReviewInstance в результаты. |
|[Создание объекта accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создайте новый accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление объекта accessReviewScheduleDefinition с указанным **идентификатором**. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта accessReviewScheduleDefinition с указанным **идентификатором**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызывающий пользователь является рецензентом в одном или нескольких экземплярах.|

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :------------------| :-------------- | :---------- |
| additionalNotificationRecipients   |[Коллекция accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md)| Определяет список дополнительных пользователей или участников группы, которые будут получать уведомления о ходе проверки доступа. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Пользователь, создавший эту проверку. Только для чтения. |
| createdDateTime  |DateTimeOffset  | Метка времени создания ряда проверки доступа. Поддерживает `$select`. Только для чтения. |
| descriptionForAdmins  |Строка  |  Описание, предоставленное авторами проверки, чтобы предоставить администраторам дополнительный контекст проверки. Поддерживает `$select`. |
| descriptionForReviewers |Строка | Описание, предоставленное авторами проверки, чтобы предоставить рецензентам дополнительный контекст проверки. Рецензенты будут видеть это описание в сообщении электронной почты, отправляемом им с запросом на проверку. Уведомления по электронной почте поддерживают до 256 символов. Поддерживает `$select`. |
| displayName | Строка   | Имя серии проверки доступа. Поддерживает `$select` и `$orderBy`. Требуется при создании. |
| fallbackReviewers   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей рецензента используется для определения списка резервных рецензентов. Эти резервные рецензенты будут получать уведомления о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует. См [. accessReviewReviewerScope](accessreviewreviewerscope.md). Заменяет **backupReviewers**. Поддерживает `$select`. <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства будет игнорироваться, если резервные рецензенты назначаются через **свойство stageSettings** . |
| id | String | Уникальный идентификатор проверки доступа, назначаемого компонентом. Поддерживает `$select`. Только для чтения.|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Это свойство необходимо при проверке доступа гостевых пользователей во всех группах Microsoft 365 и определяет, какие группы Microsoft 365 проверяются. Каждая группа станет уникальным **объектом accessReviewInstance** серии проверки доступа.  Сведения о поддерживаемых областях см. [в разделе accessReviewScope](accessreviewscope.md). Поддерживает `$select`. Примеры параметров настройки instanceEnumerationScope см. в разделе "Настройка области определения проверки доступа с помощью microsoft [API Graph"](/graph/accessreviews-scope-concept). |
| instances |[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|  Набор экземпляров проверок доступа для этой серии проверок доступа. Проверки доступа, которые не повторялись, будут иметь только один экземпляр; в противном случае имеется экземпляр для каждого повторения. |
| lastModifiedDateTime | DateTimeOffset   | Метка времени последнего изменения ряда проверки доступа. Поддерживает `$select`. Только для чтения.|
| Авторам   |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей проверки доступа используется для определения рецензентов. Свойство рецензентов можно обновить только в том случае, если отдельные пользователи назначены рецензентами. Требуется при создании. Поддерживает `$select`. Примеры параметров назначения рецензентов см. в статье "Назначение рецензентов определению проверки доступа с [помощью microsoft API Graph"](/graph/accessreviews-reviewers-concept). <br/><br/>**ПРИМЕЧАНИЕ:** Значение этого свойства будет игнорироваться, если рецензенты назначаются через **свойство stageSettings** .  |
| область  |[accessReviewScope](../resources/accessreviewscope.md)  | Определяет сущности, доступ к которых проверяется. Сведения о поддерживаемых областях см. [в разделе accessReviewScope](accessreviewscope.md). Требуется при создании. Поддерживает и `$select` `$filter` (`contains` только). Примеры параметров настройки области см. в статье "Настройка области определения проверки доступа с помощью microsoft [API Graph"](/graph/accessreviews-scope-concept). |
|stageSettings|[Коллекция accessReviewStageSettings](../resources/accessreviewstagesettings.md)| Требуется только для многоэтабной проверки доступа для определения этапов и их параметров. Каждый экземпляр проверки можно разбить на три последовательных этапа, где каждый этап может иметь отдельный набор рецензентов, резервных рецензентов и параметров. Этапы будут создаваться последовательно на основе свойства **dependsOn** . Необязательное.  <br/><br/>Если это свойство определено, его параметры используются вместо соответствующих параметров в объекте [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) и его **параметров, рецензентов** и **свойств fallbackReviewers**.  |
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Параметры для ряда проверки доступа см. определение типа ниже. Поддерживает `$select`. Требуется при создании. |
| status  |String   | Это поле только для чтения указывает состояние проверки доступа. Типичные состояния: `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, , `Completed`, и `AutoReviewed``AutoReviewing`.  <br>Поддерживает , `$select``$orderby`и `$filter` (`eq`только). Только для чтения. |
| backupReviewers (не рекомендуется) |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Эта коллекция областей рецензента используется для определения списка резервных рецензентов. Эти резервные рецензенты будут получать уведомления о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует.  Поддерживает `$select`. <br>**Примечание:** Это свойство заменено **на fallbackReviewers**. Однако указание **backupReviewers** или **fallbackReviewers** автоматически заполняет те же значения другим свойством. |


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `instances`               |[Коллекция accessReviewInstance](accessreviewinstance.md)         | Если это `accessReviewScheduleDefinition` повторяющаяся проверка доступа, экземпляры представляют каждое повторение. Повторная проверка будет иметь только один экземпляр. Экземпляры также представляют каждый уникальный ресурс, проверяемого в `accessReviewScheduleDefinition`. Если проверка содержит несколько ресурсов и несколько экземпляров, каждый ресурс будет иметь уникальный экземпляр для каждого повторения. |

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
