---
title: Создание personName
description: Используйте этот API, чтобы создать новое имя пользователя в профиле пользователя.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a63d3d200617d8bf696bf637c9a0dfa2a383662d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135238"
---
# <a name="create-personname"></a>Создание personName

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API для создания нового [объекта personName](../resources/personname.md) в профиле [пользователя.](../resources/profile.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Приложение                            | User.ReadBasic.All, User.Read.All, User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           |Описание                  |
|:---------------|:----------------------------|
| Авторизация  | Bearer {token}. Обязательный.   |
| Content-Type   | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [personName.](../resources/personname.md)

В следующей таблице показаны свойства, которые можно установить при создании [объекта personName.](../resources/personname.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|Строка|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|displayName|Строка|Предоставляет упорядоченную отрисовку firstName и lastName в зависимости от локализа пользователя или устройства.|
|во-первых|Строка|Имя пользователя.|
|id|Строка|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|initials|String|Инициалы пользователя.|
|LanguageTag|Строка|Содержит имя языка (en-US, no-NB, ru-AU) в формате IETF BCP47.   |
|последний|Строка|Фамилия пользователя.|
|maiden|Строка|Девичья фамилия пользователя. |
|средний|Строка|Среднее имя пользователя.|
|nickname|Строка|Прозвище пользователя.|
|произношение|[yomiPersonName](../resources/yomipersonname.md)|Руководство по произносить имя пользователей.|
|суффикс|Строка|Назначенные элементы, используемые после имени пользователей (например: PhD.)  |
|title|Строка|Honorifics used to prefix a users name (eg: Dr, Sir, Msam, Mrs.)|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201, Created` новый [объект personName](../resources/personname.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personname-from-profilev2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-personname-from-profilev2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-personname-from-profilev2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": null,
  "suffix": null,
  "title": null,
  "pronunciation": null
}
```


