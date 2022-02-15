---
title: Как получить фотографию группы
description: Вы можете получить фотографию (изображение) для группы.
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f6ba5b3aa527a286167aacfd78547376330a2750
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804957"
---
# <a name="get-team-photo"></a>Как получить фотографию группы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить фотографию (изображение) для группы или метаданные этой фотографии.

Действуя этим методом, мы сначала пробуем извлечь указанную фотографию из Microsoft 365. Если фотография недоступна в Microsoft 365, производится попытка извлечь ее из Azure Active Directory.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All** |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Application | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All**  |

[!INCLUDE [teamwork-permissions-note](../../../includes/teamwork-permissions-note.md)]

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос

### <a name="get-the-metadata-of-the-photo"></a>Как получить метаданные фотографии

Эта конечная точка возвращает метаданные фотографии.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
```

### <a name="get-the-photo"></a>Как получить фотографию

Эта конечная точка извлекает двоичные данные для фотографии.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo/$value
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Тело запроса

Текст для этого запроса указывать не нужно.

## <a name="response"></a>Отклик

### <a name="response-for-getting-the-metadata-of-a-photo"></a>Отклик при получении метаданных фотографии

При успешной отправке запроса этим способом возвращаются код отклика`200 OK` и метаданные о запрашиваемой фотографии.

### <a name="response-for-getting-the-photo"></a>Отклик при получении фотографии

При успешной отправке запроса этим способом возвращаются код отклика `200 OK` и двоичные данные запрашиваемой фотографии.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-photo-metadata"></a>Пример 1. Как получить метаданные фотографии

#### <a name="request"></a>Запрос

Ниже приведен пример запроса на получение метаданных фотографии группы.

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-the-team-photos-binary-data"></a>Пример 2. Получение двоичных данных фотографии команды.

Вот пример запроса для получения двоичных данных фотографии команды.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/$value
```

#### <a name="response"></a>Отклик

Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->