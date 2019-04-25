---
title: Тип ресурса Акцессревиев
description: 'В функции проверки доступа Azure AD — это `accessReview` представление доступа.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cb5d32a8dcc6b12330aca6e831a8ab2083759df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544117"
---
# <a name="accessreview-resource-type"></a>Тип ресурса Акцессревиев

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции проверки [доступа](accessreviews-root.md) Azure AD — это `accessReview` представление доступа.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Акцессревиев](../api/accessreview-get.md) |   [Акцессревиев](accessreview.md) |   Получение проверки доступа с определенным идентификатором. |
|[Создание Акцессревиев](../api/accessreview-create.md) | [Акцессревиев](accessreview.md) |   Создание нового Акцессревиев. |
|[Удаление Акцессревиев](../api/accessreview-delete.md) | Нет.   | Удаление Акцессревиев. |
|[Обновление Акцессревиев](../api/accessreview-update.md) | [Акцессревиев](accessreview.md) | Обновление Акцессревиев. |
|[Список рецензентов Акцессревиев](../api/accessreview-listreviewers.md) |      Коллекция [userIdentity](useridentity.md)| Получение рецензентов объекта Акцессревиев. |
|[Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющего в объект Акцессревиев. |
|[Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Нет.  |   Удаление проверяющего из Акцессревиев. |
|[Список решений Акцессревиев](../api/accessreview-listdecisions.md) |      Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| Получение решений для Акцессревиев.|
|[Список моих решений Акцессревиев](../api/accessreview-listmydecisions.md) |     Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| В качестве проверяющего получите мое решение Акцессревиев.|
|[Отправка напоминания о Акцессревиев](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание рецензентам Акцессревиев. |
|[Остановить Акцессревиев](../api/accessreview-stop.md) |     Нет.   |   Остановка Акцессревиев. |
|[Сброс решений Акцессревиев](../api/accessreview-reset.md) |     Нет.   |   Сброс решений во время выполнения Акцессревиев.|
|[Применение решений Акцессревиев](../api/accessreview-apply.md) |     Нет.   |   Применение решений из завершенной Акцессревиев.|

## <a name="permissions"></a>Разрешения

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | Уникальный идентификатор проверки доступа, назначенный компоненту. |
| `displayName`             |`String`                                                        | Имя проверки доступа. Требуется при создании. |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время, когда выполняется запланированное начало проверки.  Это может быть Дата в будущем.  Требуется при создании. |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время окончания запланированного рассмотрения. Это должен быть по крайней мере один день позже даты начала.  Требуется при создании. |
| `status`                  |`String`                                                        | В этом поле, доступном только для чтения, указывается состояние Акцессревиев. Типичные состояния: `Initializing`, `NotStarted` `Starting``InProgress` `Completing`,,,, `Completed`, `AutoReviewing`и `AutoReviewed`. |
| `description`             |`String`                                                        | Описание, предоставленное создателем проверки доступа, которое будет отображаться для рецензентов. |
| `businessFlowTemplateId`  |`String`                                                        | Идентификатор шаблона рабочего процесса. Требуется при создании. |
| `reviewerType`            |`String`                                                        | Тип отношения проверяющего к целевому объекту, один из `self` `delegated` или. `entityOwners` Требуется при создании. | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | Пользователь, создавший эту проверку. |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Объект, для которого проверки доступа просматривают назначения прав доступа. Это может быть группа для проверки членства пользователей в группе или приложения для проверки назначений пользователей в приложении. Требуется при создании. | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | Параметры Акцессревиев, см. |



## <a name="relationships"></a>Связи




| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
| `reviewers`               |Коллекция [userIdentity](useridentity.md)                     | Коллекция проверяющих для проверки доступа, если тип `delegate`проверки доступа ревиевертипе имеет значение. |
| `decisions`               |Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | Коллекция решений для этой проверки доступа. |
| `myDecisions`             |Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | Коллекция решений для вызывающего абонента, если вызывающий абонент является проверяющим. |
| `instances`               |Коллекция [акцессревиев](accessreview.md)         | Коллекция просмотров Access, прошедший, присутствующую и будущей, если этот объект является повторяющейся проверкой доступа. |

Независимо от того, есть ли эти связи в объекте, зависит от того, является ли объект одновременной проверкой, серией повторяющихся проверок доступа или экземпляром повторяющейся проверки доступа.

| Сценарий | Имеются рецензенты? | Принимает решения и МидеЦисионс? | Содержит экземпляры? |
|:---------|:---------------|:---------------|:---------------|
|Проверка одноразового доступа|Да | Да, после запуска | Нет |
| Обзор повторяющихся сведений о доступе | Да | Нет | Да |
| Экземпляр повторяющейся проверки доступа | Да | Да, после запуска | Нет |

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса в формате JSON.

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

## <a name="the-accessreviewsettings-type"></a>Тип Акцессревиевсеттингс

`accessReviewSettings` Предоставляет дополнительные параметры при создании проверки доступа, чтобы управлять поведением компонента при запуске проверки доступа.  Этот тип имеет следующие свойства: 

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | Флаг, указывающий, включена ли отправка сообщений рецензентам и создателем рецензирования.                |
| `remindersEnabled`|`Boolean`       | Флаг, указывающий, включены ли отправку сообщений напоминаний рецензентам.       |
| `justificationRequiredOnApproval`|`Boolean` | Флаг, указывающий, требуются ли проверяющие для предоставления обоснования при проверке доступа.|
| `activityDurationInDays`|`Int64` | Количество дней, в течение которых действия пользователей отображаются для рецензентов. |
| `autoReviewEnabled`|`Boolean` | Флаг, указывающий, следует ли установить решение, если проверяющий не предоставил один из них для использования с автоматическим применением. |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | Подробные параметры, определяющие, как компонент должен устанавливать решение по проверке, для использования с автоматическим применением, описанным ниже. |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | Подробные параметры для периодичности, описанные ниже. |
| `autoApplyReviewResultsEnabled`|`Boolean` | Флаг, указывающий, включена ли возможность автоматического применения, чтобы автоматически изменить целевой ресурс доступа к объектам.  Если этот параметр не включен, пользователь должен, после завершения проверки, применить проверку доступа. |
| `accessRecommendationsEnabled`|`Boolean` | Флаг, указывающий, включены ли рекомендации для рецензентов. |



## <a name="the-autoreviewsettings-type"></a>Тип Ауторевиевсеттингс

`autoReviewSettings` Он внедряется в параметры проверки доступа и задает поведение компонента при завершении проверки доступа.  Тип имеет одно свойство, `notReviewedResult`.

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | Должно иметь один из типов `Approve`, `Deny` или `Recommendation`. |


## <a name="the-accessreviewrecurrencesettings-type"></a>Тип Акцессревиеврекурренцесеттингс

`accessReviewRecurrenceSettings` Он внедряется в параметры проверки доступа и указывает, что проверка доступа повторяется через регулярные промежутки времени.  Этот тип имеет следующие свойства:

| Свойство                     | Тип                                                                                                          | Описание |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | Интервал повторения, который должен быть `onetime`одним из, `weekly`, `monthly`, `quarterly`или. `annual`                                                                   |
| `recurrenceEndType`|`String` | Завершение повторения. Если это так `Never`, то отсутствует явный конец ряда повторений. Если это так `endBy`, повторение оканчивается на определенную дату. Если это так `occurrences`, ряд завершается после `recurrentCount` завершения экземпляров проверки. |
| `durationInDays`|`Int32`     | Продолжительность повторения в днях.                                                                              |
| `recurrenceCount`|`Int32`    | Количество повторений, если значение `recurrenceEndType` равно `occurrences`, или 0 в противном случае.                                                        |



<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
