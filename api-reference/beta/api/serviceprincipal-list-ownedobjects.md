---
title: 'СервицепринЦипалс: List ownedObjects'
description: Получение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dc25bf07cb8e3b41cd6732653456c0af47999860
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410198"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="74cb3-104">СервицепринЦипалс: List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="74cb3-104">servicePrincipals: List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74cb3-105">Получение списка объектов, принадлежащих servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="74cb3-105">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="74cb3-106">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="74cb3-106">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="74cb3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74cb3-107">Permissions</span></span>
<span data-ttu-id="74cb3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74cb3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74cb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74cb3-110">Permission type</span></span>      | <span data-ttu-id="74cb3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74cb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74cb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74cb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74cb3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74cb3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74cb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74cb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74cb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74cb3-115">Not supported.</span></span>    |
|<span data-ttu-id="74cb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74cb3-116">Application</span></span> | <span data-ttu-id="74cb3-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74cb3-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74cb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74cb3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74cb3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74cb3-119">Optional query parameters</span></span>
<span data-ttu-id="74cb3-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="74cb3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74cb3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74cb3-121">Request headers</span></span>
| <span data-ttu-id="74cb3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="74cb3-122">Name</span></span>       | <span data-ttu-id="74cb3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="74cb3-123">Type</span></span> | <span data-ttu-id="74cb3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="74cb3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74cb3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="74cb3-125">Authorization</span></span>  | <span data-ttu-id="74cb3-126">string</span><span class="sxs-lookup"><span data-stu-id="74cb3-126">string</span></span>  | <span data-ttu-id="74cb3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74cb3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74cb3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74cb3-129">Request body</span></span>
<span data-ttu-id="74cb3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74cb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74cb3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="74cb3-131">Response</span></span>

<span data-ttu-id="74cb3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74cb3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74cb3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="74cb3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74cb3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="74cb3-134">Request</span></span>
<span data-ttu-id="74cb3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74cb3-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74cb3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="74cb3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74cb3-137">C#</span><span class="sxs-lookup"><span data-stu-id="74cb3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74cb3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74cb3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74cb3-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74cb3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="74cb3-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="74cb3-140">Response</span></span>
<span data-ttu-id="74cb3-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74cb3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
