---
title: 'orgContact: checkMemberGroups'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 97e6ce54099301600a0343fe837b947bb0ac18dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055584"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="0d0e5-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0d0e5-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="0d0e5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d0e5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="0d0e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d0e5-106">Permissions</span></span>
<span data-ttu-id="0d0e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d0e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d0e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d0e5-109">Permission type</span></span>      | <span data-ttu-id="0d0e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d0e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d0e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d0e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d0e5-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d0e5-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d0e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d0e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d0e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-114">Not supported.</span></span>    |
|<span data-ttu-id="0d0e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d0e5-115">Application</span></span> | <span data-ttu-id="0d0e5-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d0e5-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d0e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d0e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="0d0e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d0e5-118">Request headers</span></span>
| <span data-ttu-id="0d0e5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0d0e5-119">Name</span></span>       | <span data-ttu-id="0d0e5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0d0e5-120">Type</span></span> | <span data-ttu-id="0d0e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0d0e5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d0e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d0e5-122">Authorization</span></span>  | <span data-ttu-id="0d0e5-123">string</span><span class="sxs-lookup"><span data-stu-id="0d0e5-123">string</span></span>  | <span data-ttu-id="0d0e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d0e5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d0e5-126">Request body</span></span>
<span data-ttu-id="0d0e5-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d0e5-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d0e5-128">Parameter</span></span>    | <span data-ttu-id="0d0e5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0d0e5-129">Type</span></span>   |<span data-ttu-id="0d0e5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0d0e5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d0e5-131">groupIds</span><span class="sxs-lookup"><span data-stu-id="0d0e5-131">groupIds</span></span>|<span data-ttu-id="0d0e5-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d0e5-132">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="0d0e5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d0e5-133">Response</span></span>

<span data-ttu-id="0d0e5-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d0e5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0d0e5-135">Example</span></span>
<span data-ttu-id="0d0e5-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0d0e5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d0e5-137">Request</span></span>
<span data-ttu-id="0d0e5-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d0e5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d0e5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0d0e5-140">C#</span><span class="sxs-lookup"><span data-stu-id="0d0e5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d0e5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d0e5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d0e5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d0e5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d0e5-143">Java</span><span class="sxs-lookup"><span data-stu-id="0d0e5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0d0e5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d0e5-144">Response</span></span>
<span data-ttu-id="0d0e5-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-145">Here is an example of the response.</span></span> <span data-ttu-id="0d0e5-146">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0d0e5-146">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


