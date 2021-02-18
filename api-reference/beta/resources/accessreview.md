---
title: Тип ресурса accessReview
description: 'В функции проверки доступа Azure AD проверка доступа представляет `accessReview` проверку доступа.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: da155d49eedf03cdc935eeefc6b6808847176a41
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292716"
---
# <a name="accessreview-resource-type"></a>Тип ресурса accessReview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Представляет проверку доступа Azure [AD.](accessreviews-root.md)  

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviews](../api/accessreview-list.md) | [Коллекция accessReview](accessreview.md) | Список accessReviews для businessFlowTemplate. |
|[Get accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите отзыв о доступе с определенным идом. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создайте новый accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удаление accessReview. |
|[Список рецензентов accessReview](../api/accessreview-listreviewers.md) | [Коллекция userIdentity](useridentity.md)|  Получите проверяющих accessReview. |
|[Добавление рецензента accessReview](../api/accessreview-addreviewer.md) | Нет.    |   Добавление рецензента в accessReview. |
|[Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет. |    Удаление рецензента из accessReview. |
|[Список решений accessReview](../api/accessreview-listdecisions.md) | [Коллекция accessReviewDecision](accessreviewdecision.md) | Получите решения accessReview. |
|[Список решений accessReview](../api/accessreview-listmydecisions.md) | [Коллекция accessReviewDecision](accessreviewdecision.md) | Как рецензент получите мои решения по accessReview. |
|[Отправка напоминания accessReview](../api/accessreview-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) | Нет. | Остановите accessReview. |
|[Сброс решений accessReview](../api/accessreview-reset.md) | Нет.   |   Сброс решений в ходе выполнения accessReview. |
|[Применение решений accessReview](../api/accessreview-apply.md) | Нет. | Применение решений из завершенного accessReview. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | String | Уникальный идентификатор проверки доступа, назначенного функции. |
| displayName | String | Имя проверки доступа. Требуется при создании. |
| startDateTime | DateTimeOffset | Дата и время начала проверки.  Это может быть дата в будущем.  Требуется при создании. |
| endDateTime | DateTimeOffset | Дата и время окончания проверки. Это должно быть по крайней мере на день позже даты начала.  Требуется при создании. |
| status | String | Это поле, доступное только для чтения, указывает состояние accessReview. Типичные состояния: `Initializing` , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| description | String | Описание, предоставленное автором проверки доступа, чтобы показать рецензентам. |
| businessFlowTemplateId | String | Идентификатор шаблона бизнес-потока. Требуется при создании.  Это значение с чувствительностью к делу. |
| reviewerType | String | Тип отношения проверяемого с целевым объектом, одним из `self` или `delegated` `entityOwners` . Требуется при создании. | 
| createdBy | [userIdentity](useridentity.md) | Пользователь, создавший этот отзыв. |
| reviewedEntity | [identity](identity.md) | Объект, для которого проверяется доступ, просматривает назначения прав доступа. Это может быть группа для просмотра членства пользователей в группе или приложение для просмотра назначений пользователей приложению. Требуется при создании. | 
| параметры | [accessReviewSettings](accessreviewsettings.md) | Параметры accessReview см. ниже в определении типа. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| рецензенты | [Коллекция userIdentity](useridentity.md) | Коллекция рецензентов для проверки доступа, если тип reviewerType для проверки `delegated` доступа. |
| decisions | [Коллекция accessReviewDecision](accessreviewdecision.md) | Коллекция решений для этой проверки доступа. |
| myDecisions | [Коллекция accessReviewDecision](accessreviewdecision.md) | Коллекция решений для вызываемого, если вызываемая является рецензентом. |
| instances | [Коллекция accessReview](accessreview.md) | Коллекция экземпляров проверки доступа, прошедших, присутствующих и будущих, если этот объект является повторяющимся обзором доступа. |

То, присутствуют ли эти связи в объекте, зависит от того, является ли объект одноразовой проверкой доступа, серию повторяющихся отзывов о доступе или экземпляром повторяющегося анализа доступа.

| Сценарий | Есть рецензенты? | Есть ли решения и myDecisions? | Есть ли экземпляры? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Разовая проверка доступа | Да | Да, после начала работы | Нет |
| Проверка повторяющегося доступа | Да | Нет | Да |
| Экземпляр проверки повторяющегося доступа | Да | Да, после начала работы | Нет |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
 "reviewedEntity": {"@odata.type": "microsoft.graph.identity"},
 "settings": {"@odata.type": "microsoft.graph.accessReviewSettings"},
 "reviewers": [{"@odata.type": "microsoft.graph.userIdentity"}]
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


