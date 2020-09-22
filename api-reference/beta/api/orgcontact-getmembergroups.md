---
title: 'orgContact: getMemberGroups'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ef812c61b62217a857fb6d7e9a5a339fbbf1477
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979842"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="01bfa-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="01bfa-104">orgContact: getMemberGroups</span></span>

<span data-ttu-id="01bfa-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01bfa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="01bfa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01bfa-106">Permissions</span></span>
<span data-ttu-id="01bfa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01bfa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01bfa-109">Permission type</span></span>      | <span data-ttu-id="01bfa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01bfa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01bfa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01bfa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01bfa-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01bfa-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01bfa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01bfa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01bfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01bfa-114">Not supported.</span></span>    |
|<span data-ttu-id="01bfa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01bfa-115">Application</span></span> | <span data-ttu-id="01bfa-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bfa-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01bfa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01bfa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="01bfa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01bfa-118">Request headers</span></span>
| <span data-ttu-id="01bfa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="01bfa-119">Name</span></span>       | <span data-ttu-id="01bfa-120">Тип</span><span class="sxs-lookup"><span data-stu-id="01bfa-120">Type</span></span> | <span data-ttu-id="01bfa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01bfa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01bfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01bfa-122">Authorization</span></span>  | <span data-ttu-id="01bfa-123">string</span><span class="sxs-lookup"><span data-stu-id="01bfa-123">string</span></span>  | <span data-ttu-id="01bfa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01bfa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01bfa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01bfa-126">Request body</span></span>
<span data-ttu-id="01bfa-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="01bfa-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01bfa-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="01bfa-128">Parameter</span></span>    | <span data-ttu-id="01bfa-129">Тип</span><span class="sxs-lookup"><span data-stu-id="01bfa-129">Type</span></span>   |<span data-ttu-id="01bfa-130">Описание</span><span class="sxs-lookup"><span data-stu-id="01bfa-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01bfa-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="01bfa-131">securityEnabledOnly</span></span>|<span data-ttu-id="01bfa-132">Логическое</span><span class="sxs-lookup"><span data-stu-id="01bfa-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="01bfa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bfa-133">Response</span></span>

<span data-ttu-id="01bfa-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01bfa-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01bfa-135">Пример</span><span class="sxs-lookup"><span data-stu-id="01bfa-135">Example</span></span>
<span data-ttu-id="01bfa-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="01bfa-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01bfa-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="01bfa-137">Request</span></span>
<span data-ttu-id="01bfa-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01bfa-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01bfa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="01bfa-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="01bfa-140">C#</span><span class="sxs-lookup"><span data-stu-id="01bfa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01bfa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01bfa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01bfa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01bfa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="01bfa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bfa-143">Response</span></span>
<span data-ttu-id="01bfa-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01bfa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


