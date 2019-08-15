---
title: 'orgContact: getMemberGroups'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2a560d6274c6bc61a263988c981ac3ff311645b5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414303"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="de73c-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="de73c-104">orgContact: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="de73c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de73c-105">Permissions</span></span>
<span data-ttu-id="de73c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de73c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de73c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de73c-108">Permission type</span></span>      | <span data-ttu-id="de73c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de73c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de73c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de73c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de73c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de73c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de73c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de73c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de73c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de73c-113">Not supported.</span></span>    |
|<span data-ttu-id="de73c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de73c-114">Application</span></span> | <span data-ttu-id="de73c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de73c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de73c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de73c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="de73c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de73c-117">Request headers</span></span>
| <span data-ttu-id="de73c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="de73c-118">Name</span></span>       | <span data-ttu-id="de73c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="de73c-119">Type</span></span> | <span data-ttu-id="de73c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de73c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="de73c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de73c-121">Authorization</span></span>  | <span data-ttu-id="de73c-122">string</span><span class="sxs-lookup"><span data-stu-id="de73c-122">string</span></span>  | <span data-ttu-id="de73c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de73c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de73c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de73c-125">Request body</span></span>
<span data-ttu-id="de73c-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="de73c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="de73c-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="de73c-127">Parameter</span></span>    | <span data-ttu-id="de73c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="de73c-128">Type</span></span>   |<span data-ttu-id="de73c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="de73c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de73c-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="de73c-130">securityEnabledOnly</span></span>|<span data-ttu-id="de73c-131">Логическое</span><span class="sxs-lookup"><span data-stu-id="de73c-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="de73c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de73c-132">Response</span></span>

<span data-ttu-id="de73c-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de73c-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de73c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="de73c-134">Example</span></span>
<span data-ttu-id="de73c-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="de73c-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de73c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="de73c-136">Request</span></span>
<span data-ttu-id="de73c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de73c-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de73c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="de73c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de73c-139">C#</span><span class="sxs-lookup"><span data-stu-id="de73c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de73c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de73c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de73c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="de73c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de73c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="de73c-142">Response</span></span>
<span data-ttu-id="de73c-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de73c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
