---
title: Создание сертификатов
description: Создание нового объекта сертификации.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6886aab7793d0e24abb9aaf58518f7a783cb6795
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027942"
---
# <a name="create-personcertification"></a>Создание personCertification
Пространство имен: microsoft.graph

Создайте новый [объект personCertification](../resources/personcertification.md) в профиле [пользователя.](../resources/profile.md)

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
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [personCertification.](../resources/personcertification.md)

В следующей таблице показаны свойства, которые можно установить при создании нового объекта [personCertification](../resources/personcertification.md) в профиле [пользователя.](../resources/profile.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|Строка|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|certificationId  |Строка      |Справочный идентификатор для сертификации. |
|description      |Строка      |Описание сертификации.                   |
|displayName      |Строка      |Название сертификата.                         |
|endDate          |Date        |Дата истечения срока сертификации.            |
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|issuedDate       |Дата        |Дата выдачи сертификата.         |
|issuingAuthority |String      |Орган, который предоставил сертификацию.          |
|issuingCompany   |Строка      |Орган, который предоставил сертификацию.          |
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|startDate        |Date        |Дата, когда сертификация стала допустимой.       |
|thumbnailUrl     |String      |URL-адрес, ссылающийся на эскиз сертификата.   |
|webUrl           |String      |URL-адрес, ссылающийся на сертификацию.                  |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект personCertification](../resources/personcertification.md) в тексте ответа.

## <a name="examples"></a>Примеры

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personCertification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/certifications
Content-Type: application/json

{
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personcertification-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personcertification-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personcertification-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personcertification-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-personcertification-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": null,
  "issuingCompany": null,
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```


