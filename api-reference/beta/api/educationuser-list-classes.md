---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 46673a46d125bfebe1d3061b15161cf3a548a712
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441214"
---
# <a name="list-classes"></a><span data-ttu-id="b74dc-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="b74dc-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b74dc-105">Получение списка объектов курсов.</span><span class="sxs-lookup"><span data-stu-id="b74dc-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="b74dc-106">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="b74dc-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="b74dc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b74dc-107">Permissions</span></span>
<span data-ttu-id="b74dc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b74dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b74dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b74dc-110">Permission type</span></span>      | <span data-ttu-id="b74dc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b74dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b74dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b74dc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b74dc-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b74dc-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b74dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b74dc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b74dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b74dc-115">Not supported.</span></span>  |
|<span data-ttu-id="b74dc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b74dc-116">Application</span></span> | <span data-ttu-id="b74dc-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b74dc-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b74dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b74dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b74dc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b74dc-119">Optional query parameters</span></span>
<span data-ttu-id="b74dc-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b74dc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b74dc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b74dc-121">Request headers</span></span>
| <span data-ttu-id="b74dc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b74dc-122">Header</span></span>       | <span data-ttu-id="b74dc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b74dc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b74dc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b74dc-124">Authorization</span></span>  | <span data-ttu-id="b74dc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b74dc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b74dc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b74dc-127">Request body</span></span>
<span data-ttu-id="b74dc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b74dc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b74dc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b74dc-129">Response</span></span>
<span data-ttu-id="b74dc-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b74dc-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b74dc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b74dc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b74dc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b74dc-132">Request</span></span>
<span data-ttu-id="b74dc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b74dc-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b74dc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b74dc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b74dc-135">C#</span><span class="sxs-lookup"><span data-stu-id="b74dc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b74dc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b74dc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b74dc-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b74dc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b74dc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b74dc-138">Response</span></span>
<span data-ttu-id="b74dc-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b74dc-139">The following is an example of the response.</span></span> 

><span data-ttu-id="b74dc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b74dc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
