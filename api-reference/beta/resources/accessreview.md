---
title: Тип ресурса Акцессревиев
description: 'В функции проверки доступа Azure AD — это `accessReview` представление доступа.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a63291d9cefb1b6a0c249b09a95430303b3597d
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330177"
---
# <a name="accessreview-resource-type"></a>Тип ресурса Акцессревиев

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет [проверку доступа](accessreviews-root.md)Azure AD.  

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Акцессревиевс](../api/accessreview-list.md) | Коллекция [акцессревиев](accessreview.md) | Список Акцессревиевс для Бусинессфловтемплате. |
|[Получение Акцессревиев](../api/accessreview-get.md) |   [акцессревиев](accessreview.md) |   Получение проверки доступа с определенным идентификатором. |
|[Создание Акцессревиев](../api/accessreview-create.md) | [акцессревиев](accessreview.md) |   Создание нового Акцессревиев. |
|[Обновление Акцессревиев](../api/accessreview-update.md) | [акцессревиев](accessreview.md) | Обновление Акцессревиев. |
|[Удаление Акцессревиев](../api/accessreview-delete.md) | Нет.   | Удаление Акцессревиев. |
|[Список рецензентов Акцессревиев](../api/accessreview-listreviewers.md) | Коллекция [userIdentity](useridentity.md)|  Получение рецензентов объекта Акцессревиев. |
|[Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md) | Нет.    |   Добавьте проверяющего в объект Акцессревиев. |
|[Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Нет. |    Удаление проверяющего из Акцессревиев. |
|[Список решений Акцессревиев](../api/accessreview-listdecisions.md) | Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | Получение решений для Акцессревиев. |
|[Список моих решений Акцессревиев](../api/accessreview-listmydecisions.md) | Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | В качестве проверяющего получите мое решение Акцессревиев. |
|[Отправка напоминания о Акцессревиев](../api/accessreview-sendreminder.md) | Нет. | Отправьте напоминание рецензентам Акцессревиев. |
|[Остановить Акцессревиев](../api/accessreview-stop.md) | Нет. | Остановка Акцессревиев. |
|[Сброс решений Акцессревиев](../api/accessreview-reset.md) | Нет.   |   Сброс решений во время выполнения Акцессревиев. |
|[Применение решений Акцессревиев](../api/accessreview-apply.md) | Нет. | Применение решений из завершенной Акцессревиев. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | Строка | Уникальный идентификатор проверки доступа, назначенный компоненту. |
| displayName | Строка | Имя проверки доступа. Требуется при создании. |
| startDateTime | DateTimeOffset | Дата и время, когда выполняется запланированное начало проверки.  Это может быть Дата в будущем.  Требуется при создании. |
| endDateTime | DateTimeOffset | Дата и время окончания запланированного рассмотрения. Это должен быть по крайней мере один день позже даты начала.  Требуется при создании. |
| status | String | В этом поле, доступном только для чтения, указывается состояние Акцессревиев. Типичные состояния:,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` , `AutoReviewing` и `AutoReviewed` . |
| description | Строка | Описание, предоставленное создателем проверки доступа, которое будет отображаться для рецензентов. |
| бусинессфловтемплатеид | Строка | Идентификатор шаблона рабочего процесса. Требуется при создании.  Это значение чувствительно к регистру. |
| ревиевертипе | Строка | Тип отношения проверяющего к целевому объекту, один из `self` `delegated` или `entityOwners` . Требуется при создании. | 
| createdBy | [userIdentity](useridentity.md) | Пользователь, создавший эту проверку. |
| ревиеведентити | [identity](identity.md) | Объект, для которого проверки доступа просматривают назначения прав доступа. Это может быть группа для проверки членства пользователей в группе или приложения для проверки назначений пользователей в приложении. Требуется при создании. | 
| settings | [акцессревиевсеттингс](accessreviewsettings.md) | Параметры Акцессревиев, см. |

## <a name="relationships"></a>Отношения

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| обсужден | Коллекция [userIdentity](useridentity.md) | Коллекция проверяющих для проверки доступа, если тип проверки доступа Ревиевертипе имеет значение `delegated` . |
| решения | Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | Коллекция решений для этой проверки доступа. |
| мидеЦисионс | Коллекция [акцессревиевдеЦисион](accessreviewdecision.md) | Коллекция решений для вызывающего абонента, если вызывающий абонент является проверяющим. |
| instances | Коллекция [акцессревиев](accessreview.md) | Коллекция просмотров Access, прошедший, присутствующую и будущей, если этот объект является повторяющейся проверкой доступа. |

Независимо от того, есть ли эти связи в объекте, зависит от того, является ли объект одновременной проверкой, серией повторяющихся проверок доступа или экземпляром повторяющейся проверки доступа.

| Сценарий | Имеются рецензенты? | Принимает решения и МидеЦисионс? | Содержит экземпляры? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Проверка одноразового доступа | Да | Да, после запуска | Нет |
| Обзор повторяющихся сведений о доступе | Да | Нет | Да |
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


