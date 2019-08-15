---
title: Список доменов
description: Получение списка объектов Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3efd2f6a879343124b8a38ad804d8afd395e897f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417033"
---
# <a name="list-domains"></a><span data-ttu-id="e0c3b-103">Список доменов</span><span class="sxs-lookup"><span data-stu-id="e0c3b-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0c3b-104">Получение списка объектов Domain.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0c3b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0c3b-105">Permissions</span></span>
<span data-ttu-id="e0c3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c3b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0c3b-108">Permission type</span></span>      | <span data-ttu-id="e0c3b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0c3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0c3b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0c3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0c3b-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0c3b-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="e0c3b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0c3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0c3b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-113">Not supported.</span></span>    |
|<span data-ttu-id="e0c3b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0c3b-114">Application</span></span> | <span data-ttu-id="e0c3b-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c3b-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0c3b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0c3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0c3b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0c3b-117">Optional query parameters</span></span>
<span data-ttu-id="e0c3b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0c3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0c3b-119">Request headers</span></span>
| <span data-ttu-id="e0c3b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e0c3b-120">Name</span></span>      |<span data-ttu-id="e0c3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e0c3b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0c3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0c3b-122">Authorization</span></span>  | <span data-ttu-id="e0c3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e0c3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0c3b-125">Accept</span></span>         | <span data-ttu-id="e0c3b-126">приложение/JSON;</span><span class="sxs-lookup"><span data-stu-id="e0c3b-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0c3b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0c3b-127">Request body</span></span>
<span data-ttu-id="e0c3b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0c3b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0c3b-129">Response</span></span>

<span data-ttu-id="e0c3b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domain](../resources/domain.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0c3b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e0c3b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0c3b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0c3b-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e0c3b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c3b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0c3b-134">C#</span><span class="sxs-lookup"><span data-stu-id="e0c3b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0c3b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0c3b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0c3b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e0c3b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0c3b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0c3b-137">Response</span></span>
<span data-ttu-id="e0c3b-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0c3b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
