---
title: Перечисление учебных заведений
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3701952c8e9e6f1997ceb82b3ab378a20c29af76
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458208"
---
# <a name="list-schools"></a><span data-ttu-id="a5429-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="a5429-103">List schools</span></span>

<span data-ttu-id="a5429-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5429-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5429-105">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5429-105">Retrieve a list of schools for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5429-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5429-106">Permissions</span></span>

<span data-ttu-id="a5429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5429-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5429-109">Permission type</span></span>                        | <span data-ttu-id="a5429-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5429-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a5429-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5429-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5429-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a5429-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a5429-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5429-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5429-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5429-114">Not supported.</span></span>                              |
| <span data-ttu-id="a5429-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5429-115">Application</span></span>                            | <span data-ttu-id="a5429-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5429-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a5429-117">При использовании делегированных разрешений возвращаются только те ресурсы educationSchool, которые является членом пользователя проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a5429-117">When delegated permissions are used, only educationSchool resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5429-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5429-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5429-119">Optional query parameters</span></span>

<span data-ttu-id="a5429-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5429-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5429-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5429-121">Request headers</span></span>

| <span data-ttu-id="a5429-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5429-122">Header</span></span>        | <span data-ttu-id="a5429-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a5429-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a5429-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5429-124">Authorization</span></span> | <span data-ttu-id="a5429-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5429-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5429-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5429-127">Request body</span></span>

<span data-ttu-id="a5429-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5429-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5429-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5429-129">Response</span></span>

<span data-ttu-id="a5429-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5429-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5429-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a5429-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5429-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5429-132">Request</span></span>

<span data-ttu-id="a5429-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5429-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5429-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5429-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="a5429-135">C#</span><span class="sxs-lookup"><span data-stu-id="a5429-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5429-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5429-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5429-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5429-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5429-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5429-138">Response</span></span>

<span data-ttu-id="a5429-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5429-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a5429-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5429-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
