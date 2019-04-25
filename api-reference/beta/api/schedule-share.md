---
title: 'Расписание: общий доступ'
description: Предоставьте общий доступ к диапазону расписания с участниками расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eaa2eae082c2b50f39b4a3ac2547ca5b0135381f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537828"
---
# <a name="schedule-share"></a>Расписание: общий доступ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставьте общий доступ к диапазону [расписания](../resources/schedule.md) с участниками расписания.
Сделайте коллекции элементов [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени [расписания](../resources/schedule.md) , отображаемого указанными участниками группы, включая "сотрудники" и "руководители".
Каждый экземпляр [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md) поддерживает черновую и общую версии элемента. Черновая версия доступна для просмотра только руководителями, а общая версия доступна для просмотра сотрудниками и руководителями. Для каждого экземпляра [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени, действие Share обновляет общую версию из черновой версии, поэтому в дополнение к менеджерам сотрудники также могут просматривать самую актуальную информацию об элементе. Параметр **нотифитеам** указывает, какие сотрудники могут просматривать элемент.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы могут получать доступ к группам, которые не являются участниками.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

|Параметр                   |Тип           |Описание  |
|-----------------------|-------------------|--------------|
| Нотифитеам            |`Boolean`             |Указывает, должна ли вся группа получить видимое уведомление о данном действии или только те сотрудники, которым назначена смена. Обязательный.       |
| startDateTime         |`DateTimeOffset`   |Время начала совместного использования смен по расписанию. Обязательный.   |
| endDateTime           |`DateTimeOffset`   | Время окончания для совместного использования смены графика до.   |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
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

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
