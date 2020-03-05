---
title: 'servicePrincipal: Чеккмемберграупс'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63bf38ca44f75781bb501c0871a45e642799748c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453543"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="547dd-104">servicePrincipal: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="547dd-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="547dd-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="547dd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="547dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="547dd-106">Permissions</span></span>
<span data-ttu-id="547dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="547dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="547dd-109">Permission type</span></span>      | <span data-ttu-id="547dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="547dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="547dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="547dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="547dd-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="547dd-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="547dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="547dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="547dd-114">Not supported.</span></span>    |
|<span data-ttu-id="547dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="547dd-115">Application</span></span> | <span data-ttu-id="547dd-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="547dd-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="547dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="547dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="547dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="547dd-118">Request headers</span></span>
| <span data-ttu-id="547dd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="547dd-119">Name</span></span>       | <span data-ttu-id="547dd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="547dd-120">Type</span></span> | <span data-ttu-id="547dd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="547dd-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="547dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="547dd-122">Authorization</span></span>  | <span data-ttu-id="547dd-123">string</span><span class="sxs-lookup"><span data-stu-id="547dd-123">string</span></span>  | <span data-ttu-id="547dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="547dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="547dd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="547dd-126">Request body</span></span>
<span data-ttu-id="547dd-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="547dd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="547dd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="547dd-128">Parameter</span></span>    | <span data-ttu-id="547dd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="547dd-129">Type</span></span>   |<span data-ttu-id="547dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="547dd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="547dd-131">groupIds</span><span class="sxs-lookup"><span data-stu-id="547dd-131">groupIds</span></span>|<span data-ttu-id="547dd-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="547dd-132">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="547dd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="547dd-133">Response</span></span>

<span data-ttu-id="547dd-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="547dd-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="547dd-135">Пример</span><span class="sxs-lookup"><span data-stu-id="547dd-135">Example</span></span>
<span data-ttu-id="547dd-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="547dd-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="547dd-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="547dd-137">Request</span></span>
<span data-ttu-id="547dd-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="547dd-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="547dd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="547dd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="547dd-140">C#</span><span class="sxs-lookup"><span data-stu-id="547dd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="547dd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="547dd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="547dd-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="547dd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="547dd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="547dd-143">Response</span></span>
<span data-ttu-id="547dd-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="547dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
