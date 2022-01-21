---
title: Обновление educationSchool
description: Обновление свойств объекта educationSchool.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70502ab3ad21d6d71d9560c95e2cdef1fc5c5f98
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117662"
---
# <a name="update-educationschool"></a>Обновление educationSchool

Пространство имен: microsoft.graph

Обновление свойств объекта [educationSchool.](../resources/educationschool.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Тело запроса

В теле запроса поставляем представление JSON объекта [educationSchool.](../resources/educationschool.md)

В следующей таблице показаны свойства, необходимые при обновлении [educationSchool.](../resources/educationschool.md)

| Свойство             | Тип                                               | Описание                                                                                                                                                           |
| :------------------- | :------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName          | Строка                                             | Отображаемое имя учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                            |
| description          | String                                             | Описание учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                             |
| externalSource       | educationExternalSource                            | Источник, из которых была создана эта организация. Унаследованный от [educationOrganization](../resources/educationorganization.md). Возможные значения: `sis`, `manual`. |
| externalSourceDetail | String                                             | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                    |
| principalEmail       | String                                             | Адрес электронной почты директора.                                                                                                                                       |
| principalName        | String                                             | Имя директора.                                                                                                                                                |
| externalPrincipalId  | String                                             | Идентификатор директора в системе синхронизации.                                                                                                                                    |
| highestGrade         | String                                             | Самый старший класс.                                                                                                                                                 |
| lowestGrade          | String                                             | Самый младший класс.                                                                                                                                                  |
| schoolNumber         | String                                             | Номер школы.                                                                                                                                                        |
| externalId           | String                                             | Идентификатор учебного заведения в системе синхронизации.                                                                                                                                       |
| phone                | String                                             | Номер телефона учебного заведения.                                                                                                                                               |
| fax                  | String                                             | Номер факса учебного заведения.                                                                                                                                                 |
| createdBy            | [identitySet](../resources/identityset.md)         | Объект, который создал учебное заведение.                                                                                                                                        |
| address              | [physicalAddress](../resources/physicaladdress.md) | Адрес учебного заведения.                                                                                                                                                |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationschool-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-educationschool-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
