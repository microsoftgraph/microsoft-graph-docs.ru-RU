---
title: Обновление Акцессревиевсчедуледефинитион
description: Обновление существующего объекта Акцессревиевсчедуледефинитион для изменения одного или нескольких его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5eeed9d305c51ebd9a50e6714ba56fe4aea35d27
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000979"
---
# <a name="update-accessreviewscheduledefinition"></a>Обновление Акцессревиевсчедуледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление существующего объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) для изменения одного или нескольких его свойств.

>[!NOTE]
>Любые изменения, внесенные в Акцессревиевсчедуледефинитион, применяются только к будущим экземплярам. Не удается обновить экземпляры, запущенные в текущий момент.
>Кроме того, этот API не предназначен для обновления свойств, в том числе решений, на уровне Акцессревиевинстанце. Дополнительные сведения о экземплярах можно найти в разделе [акцессревиевинстанце](../resources/accessreviewinstance.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {токен}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.

В следующей таблице приведены свойства, принятые для обновления Акцессревиевсчедуледефинитион.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| displayName | Строка | Имя серии проверки доступа. |
| дескриптионфорадминс | Строка | Контекст проверки, предоставленной администраторам. |
| дескриптионфорревиеверс | Строка | Контекст проверки, предоставленной для рецензентов. |
| settings | [акцессревиевсчедулесеттингс](../resources/accessreviewschedulesettings.md) | Параметры ряда проверки доступа. Обратитесь к разделу [акцессревиевсчедулесеттингс](../resources/accessreviewscheduledefinition.md). |
| обсужден | Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md)|  Определяет, кто является рецензентом. Если ничего не указано, проверка является самостоятельным обзором (пользователи, Просмотрели проверку собственного доступа). Свойство рецензентов можно обновлять только в том случае, если назначены отдельные пользователи в качестве проверяющих. Обратитесь к разделу [акцессревиевревиеверскопе](../resources/accessreviewscheduledefinition.md). | 

Обратите внимание, что запрос PUT ожидает, что передается весь объект, в который включаются все доступные для записи свойства, а не только обновляемые свойства.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и без текста отклика.

## <a name="examples"></a>Примеры

Ниже приведен пример обновления displayName существующего ряда проверки доступа.

### <a name="request"></a>Запрос
В теле запроса добавьте представление новых свойств объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.


<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```

---


### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
