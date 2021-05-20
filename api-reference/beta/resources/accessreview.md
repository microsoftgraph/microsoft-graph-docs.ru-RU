---
title: тип ресурсов accessReview
description: 'В функции Обзоры доступа Azure AD представляет `accessReview` обзор доступа.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 75f844a165b8e5603f2d423a9d0a7aef17ab9186
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579290"
---
# <a name="accessreview-resource-type-deprecated"></a>тип ресурса accessReview (неподготовленный)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Представляет обзор доступа Azure [AD.](accessreviews-root.md)  

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[AccessReviews списка](../api/accessreview-list.md) | [коллекция accessReview](accessreview.md) | Список accessReviews для businessFlowTemplate. |
|[Получить accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите обзор доступа с определенным id. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создание нового accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удаление accessReview. |
|[Рецензенты списка accessReview](../api/accessreview-listreviewers.md) | [коллекция userIdentity](useridentity.md)|  Получите рецензентов accessReview. |
|[Добавление рецензента accessReview](../api/accessreview-addreviewer.md) | Нет.    |   Добавление рецензента в accessReview. |
|[Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет. |    Удаление рецензента из accessReview. |
|[Списки решений accessReview](../api/accessreview-listdecisions.md) | [accessReviewDecision](accessreviewdecision.md) collection | Получите решения accessReview. |
|[Список решений accessReview](../api/accessreview-listmydecisions.md) | [accessReviewDecision](accessreviewdecision.md) collection | Как рецензент, получите мои решения accessReview. |
|[Отправка напоминания accessReview](../api/accessreview-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) | Нет. | Остановите accessReview. |
|[Сброс решений accessReview](../api/accessreview-reset.md) | Нет.   |   Сброс решений в ходе выполнения accessReview. |
|[Применение решений accessReview](../api/accessreview-apply.md) | Нет. | Применение решений из завершенного accessReview. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | Строка | Уникальный идентификатор обзора доступа, назначенного функцией. |
| displayName | Строка | Имя обзора доступа. Требуется при создании. |
| startDateTime | DateTimeOffset | DateTime, когда планируется начать проверку.  Это может быть дата в будущем.  Требуется при создании. |
| endDateTime | DateTimeOffset | DateTime, когда проверка должна завершиться. Это должно быть по крайней мере на один день позже даты начала.  Требуется при создании. |
| status | String | Это поле только для чтения указывает состояние accessReview. Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| description | Строка | Описание, предоставленное создателем обзора доступа, чтобы показать рецензентам. |
| businessFlowTemplateId | Строка | Идентификатор шаблона бизнес-потока. Требуется при создании.  Это значение является чувствительным к делу. |
| reviewerType | Строка | Тип отношения рецензента к целевому объекту, одному из `self` или `delegated` `entityOwners` . Требуется при создании. | 
| createdBy | [userIdentity](useridentity.md) | Пользователь, создавший этот обзор. |
| reviewedEntity | [identity](identity.md) | Объект, для которого проверяется доступ, проверяет назначения прав доступа. Это может быть группа для проверки членства пользователей в группе или приложение для просмотра назначений пользователей приложению. Требуется при создании. | 
| settings | [accessReviewSettings](accessreviewsettings.md) | Параметры accessReview см. ниже определение типа. |

## <a name="relationships"></a>Отношения

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| рецензенты | [коллекция userIdentity](useridentity.md) | Коллекция рецензентов для проверки доступа, если reviewerType проверки доступа имеет тип `delegated` . |
| решения | [accessReviewDecision](accessreviewdecision.md) collection | Коллекция решений для этого обзора доступа. |
| myDecisions | [accessReviewDecision](accessreviewdecision.md) collection | Коллекция решений для вызываемого, если вызываемая является рецензентом. |
| instances | [коллекция accessReview](accessreview.md) | Коллекция отзывов о доступе проверяет экземпляры прошлых, нынешних и будущих, если этот объект является повторяющимся обзором доступа. |

Присутствуют ли эти связи на объекте, зависит от того, является ли объект одноразовой проверкой доступа, серией повторяющегося обзора доступа или экземпляром повторного обзора доступа.

| Сценарий | Есть рецензенты? | Есть решения и myDecisions? | Экземпляры? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Разовая проверка доступа | Да | Да, после начала | Нет |
| Повторяющиеся обзоры доступа | Да | Нет | Да |
| Экземпляр повторного обзора доступа | Да | Да, после начала | Нет |

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


