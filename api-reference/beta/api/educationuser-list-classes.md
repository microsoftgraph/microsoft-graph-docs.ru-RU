---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2860ecb5258d17183d6e4de5b53bafdd03b93f0
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439796"
---
# <a name="list-classes"></a><span data-ttu-id="5c144-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="5c144-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c144-105">Получение списка объектов курсов.</span><span class="sxs-lookup"><span data-stu-id="5c144-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="5c144-106">Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах.</span><span class="sxs-lookup"><span data-stu-id="5c144-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="5c144-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c144-107">Permissions</span></span>

<span data-ttu-id="5c144-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c144-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c144-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c144-110">Permission type</span></span>                        | <span data-ttu-id="5c144-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c144-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5c144-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c144-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c144-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5c144-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="5c144-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c144-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c144-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c144-115">Not supported.</span></span>                              |
| <span data-ttu-id="5c144-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c144-116">Application</span></span>                            | <span data-ttu-id="5c144-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c144-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c144-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c144-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c144-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c144-119">Optional query parameters</span></span>
<span data-ttu-id="5c144-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c144-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c144-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c144-121">Request headers</span></span>

| <span data-ttu-id="5c144-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c144-122">Header</span></span>        | <span data-ttu-id="5c144-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5c144-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5c144-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c144-124">Authorization</span></span> | <span data-ttu-id="5c144-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c144-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c144-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c144-127">Request body</span></span>

<span data-ttu-id="5c144-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c144-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c144-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c144-129">Response</span></span>

<span data-ttu-id="5c144-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c144-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c144-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5c144-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5c144-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c144-132">Request</span></span>
<span data-ttu-id="5c144-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c144-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5c144-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c144-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c144-135">C#</span><span class="sxs-lookup"><span data-stu-id="5c144-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c144-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c144-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c144-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c144-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c144-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c144-138">Response</span></span>

<span data-ttu-id="5c144-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c144-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5c144-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c144-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
