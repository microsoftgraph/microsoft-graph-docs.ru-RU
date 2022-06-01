---
title: Тип ресурса accessReview (не рекомендуется)
description: 'В Azure AD проверки доступа представляет `accessReview` проверку доступа.  '
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 353dfec671a400e87f613779f9d50a6e68845a34
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819477"
---
# <a name="accessreview-resource-type-deprecated"></a>Тип ресурса accessReview (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Представляет Azure AD [доступа](accessreviews-root.md).  

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов accessReview](../api/accessreview-list.md) | [Коллекция accessReview](accessreview.md) | Вывод списка объектов accessReview для businessFlowTemplate. |
|[Получение accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получение проверки доступа с определенным идентификатором. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создайте новый accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удаление объекта accessReview. |
|[Перечисление рецензентов accessReview](../api/accessreview-listreviewers.md) | [Коллекция userIdentity](useridentity.md)|  Получение рецензентов accessReview. |
|[Добавление рецензента accessReview](../api/accessreview-addreviewer.md) | Нет.    |   Добавление рецензента в accessReview. |
|[Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет. |    Удаление рецензента из accessReview. |
|[Вывод списка решений accessReview](../api/accessreview-listdecisions.md) | [Коллекция accessReviewDecision](accessreviewdecision.md) | Получение решений accessReview. |
|[Вывод списка решений accessReview](../api/accessreview-listmydecisions.md) | [Коллекция accessReviewDecision](accessreviewdecision.md) | Как рецензент получите мои решения о accessReview. |
|[Отправка напоминания accessReview](../api/accessreview-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) | Нет. | Остановите accessReview. |
|[Сброс решений accessReview](../api/accessreview-reset.md) | Нет.   |   Сбросьте решения в ходе выполнения accessReview. |
|[Применение решений accessReview](../api/accessreview-apply.md) | Нет. | Примените решения из завершенного accessReview. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | Строка | Уникальный идентификатор проверки доступа, назначаемого компонентом. |
| displayName | Строка | Имя проверки доступа. Требуется при создании. |
| startDateTime | DateTimeOffset | Дата и время начала проверки.  Это может быть дата в будущем.  Требуется при создании. |
| endDateTime | DateTimeOffset | Дата и время окончания проверки. Это значение должно быть по крайней мере на один день позже даты начала.  Требуется при создании. |
| status | String | Это поле только для чтения указывает состояние accessReview. Типичные состояния: `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, и `AutoReviewing``AutoReviewed`. |
| description | Строка | Описание, предоставленное создателем проверки доступа, для отображения рецензентам. |
| businessFlowTemplateId | Строка | Идентификатор шаблона бизнес-потока. Требуется при создании.  Это значение учитывает регистр. |
| reviewerType | Строка | Тип связи рецензента с целевым объектом, одним из или `self``delegated` `entityOwners`. Требуется при создании. | 
| createdBy | [userIdentity](useridentity.md) | Пользователь, создавший эту проверку. |
| reviewedEntity | [identity](identity.md) | Объект, для которого проверки доступа проверяют назначения прав доступа. Это может быть группа для проверки членства пользователей в группе или приложение для проверки назначений пользователей приложению. Требуется при создании. | 
| settings | [accessReviewSettings](accessreviewsettings.md) | Параметры accessReview см. в определении типа ниже. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| Авторам | [Коллекция userIdentity](useridentity.md) | Коллекция рецензентов для проверки доступа, если проверка доступа reviewerType имеет тип `delegated`. |
| Решения | [Коллекция accessReviewDecision](accessreviewdecision.md) | Коллекция решений для этой проверки доступа. |
| myDecisions | [Коллекция accessReviewDecision](accessreviewdecision.md) | Коллекция решений для вызывающего объекта, если вызывающий объект является рецензентом. |
| instances | [Коллекция accessReview](accessreview.md) | Коллекция экземпляров проверки доступа в прошлом, настоящем и будущем, если этот объект является повторяющейся проверкой доступа. |

Наличие этих связей в объекте зависит от того, является ли объект однофакторной проверкой доступа, серию повторяющихся проверок доступа или экземпляром повторяющейся проверки доступа.

| Сценарий | Есть рецензенты? | Есть ли решения и myDecisions? | Есть экземпляры? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Разовая проверка доступа | Да | Да, после запуска | Нет |
| Повторяющиеся проверки доступа | Да | Нет | Да |
| Экземпляр повторяющейся проверки доступа | Да | Да, после запуска | Нет |

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


