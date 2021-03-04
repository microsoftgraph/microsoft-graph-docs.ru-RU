---
title: 'orgContact: getMemberObjects'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a2c14280c80d24fdc5219bd66d8977cbeb7509d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433987"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="a07f7-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a07f7-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="a07f7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a07f7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="a07f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a07f7-106">Permissions</span></span>
<span data-ttu-id="a07f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a07f7-109">Permission type</span></span>      | <span data-ttu-id="a07f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a07f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a07f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a07f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a07f7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a07f7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a07f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a07f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a07f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a07f7-114">Not supported.</span></span>    |
|<span data-ttu-id="a07f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a07f7-115">Application</span></span> | <span data-ttu-id="a07f7-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07f7-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a07f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a07f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a07f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a07f7-118">Request headers</span></span>
| <span data-ttu-id="a07f7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a07f7-119">Name</span></span>       | <span data-ttu-id="a07f7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a07f7-120">Type</span></span> | <span data-ttu-id="a07f7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a07f7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a07f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a07f7-122">Authorization</span></span>  | <span data-ttu-id="a07f7-123">string</span><span class="sxs-lookup"><span data-stu-id="a07f7-123">string</span></span>  | <span data-ttu-id="a07f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a07f7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a07f7-126">Request body</span></span>
<span data-ttu-id="a07f7-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a07f7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a07f7-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="a07f7-128">Parameter</span></span>    | <span data-ttu-id="a07f7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a07f7-129">Type</span></span>   |<span data-ttu-id="a07f7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a07f7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a07f7-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a07f7-131">securityEnabledOnly</span></span>|<span data-ttu-id="a07f7-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="a07f7-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="a07f7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07f7-133">Response</span></span>

<span data-ttu-id="a07f7-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a07f7-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07f7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a07f7-135">Example</span></span>
<span data-ttu-id="a07f7-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a07f7-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a07f7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a07f7-137">Request</span></span>
<span data-ttu-id="a07f7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a07f7-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a07f7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a07f7-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="a07f7-140">C#</span><span class="sxs-lookup"><span data-stu-id="a07f7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a07f7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a07f7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a07f7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a07f7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a07f7-143">Java</span><span class="sxs-lookup"><span data-stu-id="a07f7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a07f7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07f7-144">Response</span></span>
<span data-ttu-id="a07f7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a07f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


