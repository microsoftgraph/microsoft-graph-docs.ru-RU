---
title: Список соглашений
description: Извлечение списка объектов соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 90d4421342a74b6d89bae2e02c9a61535ce40a29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775234"
---
# <a name="list-agreements"></a><span data-ttu-id="d0c5e-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="d0c5e-103">List agreements</span></span>

<span data-ttu-id="d0c5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0c5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0c5e-105">Извлечение списка [объектов](../resources/agreement.md) соглашения.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0c5e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c5e-106">Permissions</span></span>
<span data-ttu-id="d0c5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c5e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c5e-109">Permission type</span></span>                        | <span data-ttu-id="d0c5e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0c5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0c5e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0c5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0c5e-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0c5e-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="d0c5e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0c5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0c5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-114">Not supported.</span></span> |
|<span data-ttu-id="d0c5e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0c5e-115">Application</span></span>                            | <span data-ttu-id="d0c5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0c5e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0c5e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0c5e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d0c5e-118">Optional query parameters</span></span>
<span data-ttu-id="d0c5e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0c5e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0c5e-120">Request headers</span></span>
| <span data-ttu-id="d0c5e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d0c5e-121">Name</span></span>         | <span data-ttu-id="d0c5e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c5e-122">Type</span></span>        | <span data-ttu-id="d0c5e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c5e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d0c5e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0c5e-124">Authorization</span></span> | <span data-ttu-id="d0c5e-125">string</span><span class="sxs-lookup"><span data-stu-id="d0c5e-125">string</span></span> | <span data-ttu-id="d0c5e-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0c5e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0c5e-128">Request body</span></span>
<span data-ttu-id="d0c5e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d0c5e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c5e-130">Response</span></span>
<span data-ttu-id="d0c5e-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` соглашения в тексте отклика. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="d0c5e-131">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="d0c5e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0c5e-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d0c5e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0c5e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0c5e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0c5e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="d0c5e-135">C#</span><span class="sxs-lookup"><span data-stu-id="d0c5e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0c5e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0c5e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0c5e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0c5e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0c5e-138">Java</span><span class="sxs-lookup"><span data-stu-id="d0c5e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0c5e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c5e-139">Response</span></span>
><span data-ttu-id="d0c5e-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0c5e-140">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "Sample ToU",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
