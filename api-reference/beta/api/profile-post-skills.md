---
title: Создание СкиллпрофиЦиенци
description: Используйте этот API для создания нового СкиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1943b28688af983aa0bd78db1b18df246867962d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810064"
---
# <a name="create-skillproficiency"></a>Создание СкиллпрофиЦиенци

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API, чтобы создать новый объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. ReadWrite, User. ReadWrite. ALL          |
| Делегированные (личная учетная запись Майкрософт) | User. ReadWrite, User. ReadWrite. ALL          |
| Для приложений                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
POST /users/{id | userPrincipalName}/profile/skills
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                 |
|:---------------|:----------------------------|
| Авторизация  | Bearer {токен}. Обязательный.   |
| Content-Type   | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в формате JSON.

В следующей таблице приведены свойства, которые можно задать при создании нового объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный). |
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|displayName|String|Содержит понятное имя для навыка. |
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|навыки|скиллпрофиЦиенцилевел|Сведения о пользователях, которые подключают этот навык. Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на источник информации о навыке. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_skillproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/skills
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "allowedAudiences": "organization",
  "displayName": "API Design",
  "proficiency": "generalProfessional",
  "collaborationTags": [
    "ableToMentor"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```
