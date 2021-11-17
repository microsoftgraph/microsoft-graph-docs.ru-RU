---
title: Обновление типа ресурсов projectParticipation
description: Обновление свойств объекта projectParticipation в профиле пользователя.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 93c1b08a6c997eb27ed9cf2a0f89a41012265fe0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027858"
---
# <a name="update-projectparticipation"></a>Обновление projectparticipation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [projectParticipation](../resources/projectParticipation.md) в профиле [пользователя.](../resources/profile.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User.ReadWrite, User.ReadWrite.All          |
| Делегированные (личная учетная запись Майкрософт) | User.ReadWrite, User.ReadWrite.All          |
| Для приложений                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           |Описание                  |
|:---------------|:----------------------------|
| Авторизация  | Bearer {token}. Обязательный.   |
| Content-Type   | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|Строка|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, которые пользователь связал с проектом (например, цифровая трансформация, нефтяная вышка). |
|клиент|[companyDetail](../resources/companydetail.md)|Содержит подробные сведения о клиенте, для который был проект. |
|collaborationTags|Коллекция объектов string|Содержит теги сценариев работы, которые пользователь связал с интересом. Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .|
|коллеги|[коллекция relatedPerson](../resources/relatedperson.md)|Списки людей, которые также работали над проектом. |
|подробные|[positionDetail](../resources/positiondetail.md)|Содержит сведения о роли пользователя в проекте.|
|displayName|Строка|Содержит удобное имя для проекта.|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|спонсоры|[коллекция relatedPerson](../resources/relatedperson.md)|Лицо или люди, которые спонсировали проект.    |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект projectParticipation](../resources/projectparticipation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "allowedAudiences": "organization",
  "client": {
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-projectparticipation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-projectparticipation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
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
  "source": null,
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "pronunciation": null,
    "department": "Corporate Marketing",
    "officeLocation": null,
    "address": null,
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": null,
      "address": null,
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "endMonthYear": "datetime-value",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "startMonthYear": "datetime-value",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  },
  "colleagues": null,
  "sponsors": null
}
```


