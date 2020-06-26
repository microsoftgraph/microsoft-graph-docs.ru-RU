---
title: Как получить фотографию группы
description: Вы можете получить фотографию (изображение) для группы.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a02f0cd05c0f092fbafc584e9a74a578122f7c5
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896506"
---
# <a name="get-team-photo"></a>Как получить фотографию группы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить фотографию (изображение) для группы или метаданные этой фотографии. В целом, лучше всего сначала попробовать извлечь метаданные о размере фотографии, которую вы хотите получить, чтобы убедиться в том, что этот размер доступен. После того как вы извлекли метаданные, используйте путь `/$value`, чтобы получить двоичные данные фотографии.

Этот метод сначала предпринимает попытку получить заданную фотографию из Microsoft 365. Если фотография недоступна в Microsoft 365, она пытается получить фотографию из Azure Active Directory.

Ниже приведены поддерживаемые размеры фотографий HD в Microsoft 365:48x48, 64x64, 96x96, 120x120, 240x240, 360 x 360, 432 x 432, 504 504 и 648x648 Пиксели. Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.

Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для фотографии этого размера. Если запрашиваемый размер недоступен, вы можете получить фотографию меньшего размера. Например, если самая крупная загруженная фотография имеет размер 504 x 504 пикселя, для скачивания будут доступны все размеры этой фотографии, кроме 648 x 648. Если указанный размер недоступен в Microsoft 365 или в Azure Active Directory, то размер 1x1 возвращается с остальными метаданными.

> [!Note]
> Общий размер запроса REST не должен превышать 4 МБ. Таким образом, размер фотографии составит менее 4 МБ.

## <a name="permissions"></a>Разрешения

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Теамсеттингс. Read. Group *, теамсеттингс. Edit. Group*, Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL |

> **Note**: разрешения, помеченные как * использовать [согласие с определенным ресурсом](https://aka.ms/teams-rsc).

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос

### <a name="get-the-metadata-of-the-photo"></a>Как получить метаданные фотографии

Эта конечная точка возвращает метаданные фотографии. Если размер не указывать, возвращаются метаданные крупнейшей доступной фотографии.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a>Как получить фотографию

Эта конечная точка извлекает двоичные данные для фотографии. Если размер не указан, возвращается наибольший доступный размер.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a>Параметры пути

Для этого метода поддерживается необязательный параметр пути, позволяющий указать размер фотографии, которую нужно извлечь. Можно указать любой размер вплоть до максимального доступного. Чтобы определить максимальный доступный размер, получите метаданные фотографии.

|**Параметр**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|size  |String  | Размер фотографии. Поддерживаются следующие размеры фотографий HD в Microsoft 365:48x48, 64x64, 96x96, 120x120, 240x240, 360 x 360, 432 x 432, 504 504 и 648x648. Фотографии могут быть любого размера, если они хранятся в Azure Active Directory. Необязательный параметр.|

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {token}. Required.  |

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

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a>Пример 2. Как получить фотографию группы определенного размера

Вот пример запроса на получение фотографии группы определенного размера.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a>Отклик

Содержит двоичные данные запрошенной фотографии размера 240 х 240. Код HTTP-отклика: 200.

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
