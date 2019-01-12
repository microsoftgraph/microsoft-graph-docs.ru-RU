---
title: Тип ресурса accessReview
description: 'В Azure AD access дается обзор компонента, `accessReview` представляет проверки доступа.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6d97382957b7c61625ec54af4c572962be839b4a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950664"
---
# <a name="accessreview-resource-type"></a>Тип ресурса accessReview

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `accessReview` представляет проверки доступа.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите обзор доступа с определенным идентификатором. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создание нового accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удалите accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Список accessReview рецензентов](../api/accessreview-listreviewers.md) |      Коллекция [удостоверению пользователя](useridentity.md)| Получите рецензентов accessReview. |
|[Добавление accessReview редактор](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющий accessReview. |
|[Удаление accessReview редактор](../api/accessreview-removereviewer.md) | Нет.  |   Удаление рецензента из accessReview. |
|[Список accessReview решения](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) коллекции| Получите решения accessReview.|
|[Мои accessReview решения](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) коллекции| В качестве читателя получите Мои решения accessReview.|
|[Отправлять напоминание accessReview](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание, чтобы проверяющие accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) |     Нет.   |   Остановите accessReview. |
|[Сброс accessReview решения](../api/accessreview-reset.md) |     Нет.   |   Сброс решения, принимаемые при accessReview в хода выполнения.|
|[Применение accessReview решения](../api/accessreview-apply.md) |     Нет.   |   Применение решения из завершенных accessReview.|

## <a name="permissions"></a>Permissions

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.Read.All AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | Функция назначенный уникальный идентификатор проверки доступа. |
| `displayName`             |`String`                                                        | Имя проверки доступа. Требуется при создании. |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время при планировании проверки быть запуск.  Это может быть даты в будущем.  Требуется при создании. |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время после запланированного окончания проверки. Это должно быть более поздней, чем дата начала по крайней мере один день.  Требуется при создании. |
| `status`                  |`String`                                                        | В этом поле только для чтения указывает текущее состояние accessReview. Следующие типичные состояния `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, и `AutoReviewed`. |
| `description`             |`String`                                                        | Описание, заданное создателем проверки доступа, для отображения рецензентов. |
| `businessFlowTemplateId`  |`String`                                                        | Идентификатор шаблона потока бизнеса. Требуется при создании. |
| `reviewerType`            |`String`                                                        | Тип отношения рецензент целевой объект, один из `self`, `delegate` или `entityOwners`. Требуется при создании. | 
| `createdBy`               |[удостоверению пользователя](useridentity.md)                                 | Пользователь, создавший этот анализ. |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Объект, для которого дается обзор доступа имеет назначение прав доступа, например, членство в группах для пользователей в группу или назначения пользователей для приложения. Требуется при создании. | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | Параметры accessReview, просмотрите ниже определения типа. |



## <a name="relationships"></a>Связи




| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `reviewers`               |Коллекция [удостоверению пользователя](useridentity.md)                     | Коллекция рецензентов на проверку доступа, если reviewerType проверки доступа имеет тип `delegate`. |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md) коллекции | Коллекция решений для этой проверки доступа. |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md) коллекции | Коллекция решений для вызывающего абонента, если проверяющий вызывающего абонента. |
| `instances`               |[accessReview](accessreview.md) коллекции         | Коллекции обзоры доступа экземпляров прошлом, настоящее и будущее, если этот объект является повторяющейся проверки доступа. |

Ли связи для объекта, зависят от того, является ли объект review однократного доступа, серии повторяющихся проверки доступа или экземпляр повторяющейся проверки доступа.

| Сценарий | Имеет рецензентов? | Имеет решения и myDecisions? | Имеет экземпляры? |
|:---------|:---------------|:---------------|:---------------|
|Обзор однократного доступа|Да | Да, после запуска | Нет |
| Повторяющееся проверки доступа | Да | Нет | Да |
| Экземпляр повторяющейся проверки доступа | Да | Да, после запуска | Нет |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a>Тип accessReviewSettings

`accessReviewSettings` Предоставляет дополнительные параметры при создании проверки доступа для управления поведением компонента при запуске проверки доступа.  Этот тип имеет следующие свойства: 

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | Флаг, указывающий, включена ли отправке почты рецензентов и просмотр создателя.                |
| `remindersEnabled`|`Boolean`       | Флаг, указывающий, включены ли отправка по электронной почте напоминания для рецензентов.       |
| `justificationRequiredOnApproval`|`Boolean` | Флаг, указывающий, требуются ли рецензентов для предоставления обоснование при проверке доступа.|
| `activityDurationInDays`|`Int64` | Количество дней действия пользователя для отображения рецензентов. |
| `autoReviewEnabled`|`Boolean` | Флаг, указывающий ли компонент следует устанавливать решения, если проверяющий одно, для использования с auto-apply, не предоставил включена. |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | Подробные параметры для настроек проверки решение, для использования с auto-apply, описанные ниже, в функцию. |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | Подробные параметры для повторения, описанные ниже. |
| `autoApplyReviewResultsEnabled`|`Boolean` | Флаг, указывающий ли автоматически назначаемой включена возможность, чтобы автоматически изменить целевой объект доступа ресурс.  Если не включен, пользователь впоследствии необходимо применить изменения проверки доступа после завершения проверки доступа. |
| `accessRecommendationsEnabled`|`Boolean` | Флаг, указывающий, включено ли отображение рекомендаций рецензентов. |



## <a name="the-autoreviewsettings-type"></a>Тип autoReviewSettings

`autoReviewSettings` Встроенного в параметры проверки доступа, а также определяет поведение функции при завершении проверки доступа.  Тип имеет одно свойство `notReviewedResult`.

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | Должно иметь один из типов `Approve`, `Deny` или `Recommendation`. |


## <a name="the-accessreviewrecurrencesettings-type"></a>Тип accessReviewRecurrenceSettings

`accessReviewRecurrenceSettings` Встроенного в параметры проверки доступа и указывает, что проверка доступа повторяется через регулярные интервалы времени.  Этот тип имеет следующие свойства:

| Свойство                     | Тип                                                                                                          | Описание |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | Интервал повторения, который должен быть один из `onetime`, `weekly`, `monthly`, `quarterly` или `annual`.                                                                   |
| `recurrenceEndType`|`String` | Как повторение будет завершено. Он может иметь одно из `Never`, что нет без явного конец повторений, `Endby`, повторения заканчивается в определенной даты, и `occurrences`, заканчивается, что ряд после завершения определенное количество экземпляров просмотра. |
| `durationInDays`|`Int32`     | Продолжительность в днях для повторения.                                                                              |
| `recurrenceCount`|`Int32`    | Число повторов, если значение `recurrenceEndType` — это `occurrences`.                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
