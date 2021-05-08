---
title: Список участников образовательного класса
description: Получает преподавателей и учащихся для курса. Обратите внимание на то, что если используется делегированный маркер, участников могут видеть только другие участники курса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eadc2f00fee83f3663ab983118f92ce84f8cc607
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232094"
---
# <a name="list-members-of-an-educationclass"></a><span data-ttu-id="94400-104">Список участников образовательного класса</span><span class="sxs-lookup"><span data-stu-id="94400-104">List members of an educationClass</span></span>

<span data-ttu-id="94400-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94400-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94400-106">Извлекает [участников educationUser](../resources/educationuser.md) из [класса educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="94400-106">Retrieves the [educationUser](../resources/educationuser.md) members of an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94400-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94400-107">Permissions</span></span>
<span data-ttu-id="94400-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94400-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94400-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94400-110">Permission type</span></span>                        | <span data-ttu-id="94400-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94400-111">Permissions (from least to most privileged)</span></span>                         |
| :------------------------------------- | :------------------------------------------------------------------ |
| <span data-ttu-id="94400-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94400-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94400-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="94400-113">EduRoster.ReadBasic</span></span>                                                 |
| <span data-ttu-id="94400-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94400-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94400-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="94400-115">Not supported</span></span>                                                       |
| <span data-ttu-id="94400-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="94400-116">Application</span></span>                            | <span data-ttu-id="94400-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="94400-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> |

> [!NOTE]
> <span data-ttu-id="94400-118">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="94400-118">Note that if the delegated token is used, members can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="94400-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94400-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94400-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94400-120">Optional query parameters</span></span>

<span data-ttu-id="94400-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="94400-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="94400-122">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="94400-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="94400-123">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="94400-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="94400-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94400-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94400-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94400-125">Request headers</span></span>
| <span data-ttu-id="94400-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94400-126">Header</span></span>       | <span data-ttu-id="94400-127">Значение</span><span class="sxs-lookup"><span data-stu-id="94400-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94400-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94400-128">Authorization</span></span>  | <span data-ttu-id="94400-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94400-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94400-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94400-131">Request body</span></span>
<span data-ttu-id="94400-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94400-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94400-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="94400-133">Response</span></span>
<span data-ttu-id="94400-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="94400-134">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94400-135">Пример</span><span class="sxs-lookup"><span data-stu-id="94400-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94400-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="94400-136">Request</span></span>
<span data-ttu-id="94400-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94400-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94400-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="94400-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="c"></a>[<span data-ttu-id="94400-139">C#</span><span class="sxs-lookup"><span data-stu-id="94400-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94400-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94400-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94400-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94400-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94400-142">Java</span><span class="sxs-lookup"><span data-stu-id="94400-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94400-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="94400-143">Response</span></span>
<span data-ttu-id="94400-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94400-144">The following is an example of the response.</span></span> 

><span data-ttu-id="94400-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94400-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
