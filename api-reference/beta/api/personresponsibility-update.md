---
title: Обновление Персонреспонсибилити
description: Обновление свойств объекта Персонреспонсибилити.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 38ca672825c49f0149dcf9b06b4c57d8df92c0e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017369"
---
# <a name="update-personresponsibility"></a>Обновление Персонреспонсибилити
Пространство имен: microsoft.graph

Обновление свойств объекта [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |
| Для приложений                            | User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL                            |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [персонреспонсибилити](../resources/personresponsibility.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [персонреспонсибилити](../resources/personresponsibility.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|description|String|Описание ответственности.|
|displayName|String|Содержит понятное имя для ответственности. |
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на веб-страницу или ресурс, отвечающие за ответственность.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонреспонсибилити](../resources/personresponsibility.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


