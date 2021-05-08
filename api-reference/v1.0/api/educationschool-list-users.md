---
title: Список пользователей образовательных учреждений
description: Получение списка пользователей в учебном заведении.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37bec88be07f9dba3e91d44558508ce82004c74
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232006"
---
# <a name="list-users-of-an-educationschool"></a><span data-ttu-id="6303c-103">Список пользователей образовательных учреждений</span><span class="sxs-lookup"><span data-stu-id="6303c-103">List users of an educationSchool</span></span>

<span data-ttu-id="6303c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6303c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6303c-105">Получите ресурсы [educationUser,](../resources/educationuser.md) связанные с [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6303c-105">Get the [educationUser](../resources/educationuser.md) resources associated with an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6303c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6303c-106">Permissions</span></span>

<span data-ttu-id="6303c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6303c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6303c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6303c-109">Permission type</span></span>                        | <span data-ttu-id="6303c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6303c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6303c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6303c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6303c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6303c-112">Not supported.</span></span>                              |
| <span data-ttu-id="6303c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6303c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6303c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6303c-114">Not supported.</span></span>                              |
| <span data-ttu-id="6303c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6303c-115">Application</span></span>                            | <span data-ttu-id="6303c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6303c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6303c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6303c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6303c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6303c-118">Optional query parameters</span></span>

<span data-ttu-id="6303c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6303c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="6303c-120">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="6303c-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6303c-121">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="6303c-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6303c-122">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6303c-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6303c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6303c-123">Request headers</span></span>
| <span data-ttu-id="6303c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6303c-124">Header</span></span>       | <span data-ttu-id="6303c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6303c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6303c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6303c-126">Authorization</span></span>  | <span data-ttu-id="6303c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6303c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6303c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6303c-129">Request body</span></span>
<span data-ttu-id="6303c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6303c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6303c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6303c-131">Response</span></span>
<span data-ttu-id="6303c-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6303c-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6303c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6303c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6303c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6303c-134">Request</span></span>
<span data-ttu-id="6303c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6303c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6303c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6303c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="c"></a>[<span data-ttu-id="6303c-137">C#</span><span class="sxs-lookup"><span data-stu-id="6303c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6303c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6303c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6303c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6303c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6303c-140">Java</span><span class="sxs-lookup"><span data-stu-id="6303c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6303c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6303c-141">Response</span></span>
<span data-ttu-id="6303c-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6303c-142">The following is an example of the response.</span></span> 

><span data-ttu-id="6303c-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6303c-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
