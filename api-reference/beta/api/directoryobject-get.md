---
title: Получение объекта DirectoryObject
description: Получение свойств и связей объекта directoryobject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c125ba594e677307fd22a2d7e46a27b38d275a4d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719590"
---
# <a name="get-directoryobject"></a><span data-ttu-id="c2007-103">Получение объекта DirectoryObject</span><span class="sxs-lookup"><span data-stu-id="c2007-103">Get directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2007-104">Получение свойств и связей объекта directoryobject.</span><span class="sxs-lookup"><span data-stu-id="c2007-104">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2007-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2007-105">Permissions</span></span>
<span data-ttu-id="c2007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2007-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2007-108">Permission type</span></span>      | <span data-ttu-id="c2007-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2007-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2007-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2007-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2007-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2007-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2007-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2007-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2007-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2007-113">Not supported.</span></span>    |
|<span data-ttu-id="c2007-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2007-114">Application</span></span> | <span data-ttu-id="c2007-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2007-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2007-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2007-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2007-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2007-117">Optional query parameters</span></span>
<span data-ttu-id="c2007-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2007-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c2007-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2007-119">Request headers</span></span>
| <span data-ttu-id="c2007-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c2007-120">Name</span></span>       | <span data-ttu-id="c2007-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c2007-121">Type</span></span> | <span data-ttu-id="c2007-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2007-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2007-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2007-123">Authorization</span></span>  | <span data-ttu-id="c2007-124">string</span><span class="sxs-lookup"><span data-stu-id="c2007-124">string</span></span>  | <span data-ttu-id="c2007-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2007-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2007-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2007-127">Request body</span></span>
<span data-ttu-id="c2007-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2007-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2007-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2007-129">Response</span></span>

<span data-ttu-id="c2007-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2007-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2007-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2007-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2007-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2007-132">Request</span></span>
<span data-ttu-id="c2007-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2007-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2007-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2007-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2007-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2007-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2007-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2007-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2007-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c2007-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2007-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2007-138">Response</span></span>
<span data-ttu-id="c2007-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2007-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
