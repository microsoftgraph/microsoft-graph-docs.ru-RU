---
title: Создание публикаций
description: Создание объекта публикации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 75692418ae2d54650f4ae6c616c727fab5b040e2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819749"
---
# <a name="create-itempublication"></a>Создание элемента itemPublication
Пространство имен: microsoft.graph

Создание объекта [itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User.ReadWrite, User.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | User.ReadWrite, User.ReadWrite.All |
| Для приложений                            | User.ReadWrite.All                            |
## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [itemPublication в формате JSON.](../resources/itempublication.md)

В таблице ниже приведены свойства, которые можно установить при создании нового [объекта itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут просматривать значения, содержащиеся в сущности. Наследуется от [itemFacet.](../resources/itemfacet.md) Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя или приложения, создавшего сущность. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset, когда был создан объект. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|description    |String      |Описание публикации.                   |
|displayName    |String      |Название публикации.                         |
|id|String|Идентификатор, используемый для индивидуального адресации сущности. Наследуется от [сущности](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)|Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя или приложения, изменившего сущность. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset, когда был создан объект. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|publishedDate  |Дата        |Дата публикации публикации.      |
|publisher      |String      |Публикация или издатель для публикации.     |
|source|[personDataSource](../resources/persondatasource.md)|Где значения инициированы при синхронизации из другой службы. Наследуется от [itemFacet.](../resources/itemfacet.md)|
|thumbnailUrl   |String      |URL-адрес ссылается на эскиз публики.   |
|webUrl         |String      |URL-адрес, ссылающиеся на публикацию.                  |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект itemPublication](../resources/itempublication.md) в теле отклика.

## <a name="examples"></a>Примеры

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemPublication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/publications
Content-Type: application/json
Content-length: 497

{
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
}
-->
``` http
HTTP/1.1 201 Created
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
