---
title: 'расписание: доля'
description: Поделитесь диапазоном времени расписания с участниками расписания.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b14688102dd7f08cad8ee46f2b62fab7d9995feb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993866"
---
# <a name="schedule-share"></a>расписание: доля

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Поделитесь [диапазоном](../resources/schedule.md) времени расписания с участниками расписания.
Сделайте коллекции элементов [shift,](../resources/shift.md) [openshift](../resources/openshift.md) и [timeOff](../resources/timeoff.md) в [](../resources/schedule.md) указанном диапазоне времени для просмотра указанными участниками группы, включая сотрудников и менеджеров.
Каждая [](../resources/schedule.md) [смена, экземпляр openshift](../resources/openshift.md) и [timeOff](../resources/timeoff.md) в расписании поддерживают проектную версию и общую версию элемента. [](../resources/shift.md) Проектную версию просматривают только руководители, а общую версию просматривают сотрудники и руководители. Для [](../resources/shift.md)каждой смены, экземпляра [openshift](../resources/openshift.md) и [timeOff](../resources/timeoff.md) в указанном диапазоне времени действие share обновляет общую версию из черновиковой версии, чтобы помимо руководителей сотрудники могли просматривать наиболее актуальные сведения о элементе. Параметр **notifyTeam** далее указывает, какие сотрудники могут просматривать элемент.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.ReadWrite.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Schedule.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

|Параметр                   |Тип           |Описание  |
|-----------------------|-------------------|--------------|
| notifyTeam            |`Boolean`             |Указывает, должна ли вся команда получать видимое уведомление об этом действии, или только сотрудникам, у которых назначена смена, которая была общей. Обязательный.       |
| startDateTime         |`DateTimeOffset`   |Время начала обмена сменами в расписании. Обязательный элемент.   |
| endDateTime           |`DateTimeOffset`   | Конечный период для обмена сменами в расписании до.   |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/schedule-share-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


