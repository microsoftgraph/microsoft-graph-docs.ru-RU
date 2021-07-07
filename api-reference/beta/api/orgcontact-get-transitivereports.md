---
title: Get transitiveReports for orgContact
description: Получите количество транзитных отчетов для организационного контакта.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2ef9be3212ece4478e53dbbedbb0d2531e816dde
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316946"
---
# <a name="get-transitivereports-for-orgcontact"></a><span data-ttu-id="518ec-103">Get transitiveReports for orgContact</span><span class="sxs-lookup"><span data-stu-id="518ec-103">Get transitiveReports for orgContact</span></span>

<span data-ttu-id="518ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518ec-105">Извлечение графа транзитных отчетов для организационного контакта.</span><span class="sxs-lookup"><span data-stu-id="518ec-105">Retrieve a count of transitive reports for an organizational contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="518ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="518ec-106">Permissions</span></span>

<span data-ttu-id="518ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="518ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="518ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="518ec-109">Permission type</span></span> | <span data-ttu-id="518ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="518ec-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="518ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="518ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="518ec-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="518ec-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="518ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="518ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="518ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="518ec-114">Not supported.</span></span> |
| <span data-ttu-id="518ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="518ec-115">Application</span></span> | <span data-ttu-id="518ec-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="518ec-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="518ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="518ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/transitiveReports/$count
```

## <a name="optional-query-parameters"></a><span data-ttu-id="518ec-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="518ec-118">Optional query parameters</span></span>

<span data-ttu-id="518ec-119">Этот метод не поддерживает использование параметров запроса, но требует `$count` сегмента запросов.</span><span class="sxs-lookup"><span data-stu-id="518ec-119">This method does not support the use of query parameters, but does require the `$count` query segment.</span></span>

## <a name="request-headers"></a><span data-ttu-id="518ec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="518ec-120">Request headers</span></span>

| <span data-ttu-id="518ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="518ec-121">Header</span></span>       | <span data-ttu-id="518ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="518ec-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="518ec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="518ec-123">Authorization</span></span>  | <span data-ttu-id="518ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="518ec-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="518ec-126">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="518ec-126">ConsistencyLevel</span></span> | <span data-ttu-id="518ec-127">необязательный.</span><span class="sxs-lookup"><span data-stu-id="518ec-127">eventual.</span></span> <span data-ttu-id="518ec-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="518ec-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="518ec-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="518ec-129">Request body</span></span>

<span data-ttu-id="518ec-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="518ec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="518ec-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="518ec-131">Response</span></span>

<span data-ttu-id="518ec-132">В случае успешной работы этот метод возвращает код ответа и количество транзитных отчетов для организационного контакта `200 OK` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="518ec-132">If successful, this method returns a `200 OK` response code and a count of transitive reports for an organizational contact in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="518ec-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="518ec-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="518ec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="518ec-134">Request</span></span>

<span data-ttu-id="518ec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="518ec-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="518ec-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="518ec-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="518ec-137">C#</span><span class="sxs-lookup"><span data-stu-id="518ec-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="518ec-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="518ec-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="518ec-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="518ec-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="518ec-140">Java</span><span class="sxs-lookup"><span data-stu-id="518ec-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="518ec-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="518ec-141">Response</span></span>

<span data-ttu-id="518ec-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="518ec-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="518ec-143">5 </span><span class="sxs-lookup"><span data-stu-id="518ec-143">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
