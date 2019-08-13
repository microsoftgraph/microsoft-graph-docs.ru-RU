---
title: 'servicePrincipal: Чеккмемберграупс'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 60623e5e20f2a637f05d4d4da38a55f7f1578e5c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364112"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="787d8-104">servicePrincipal: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="787d8-104">servicePrincipal: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="787d8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="787d8-105">Permissions</span></span>
<span data-ttu-id="787d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="787d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="787d8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="787d8-108">Permission type</span></span>      | <span data-ttu-id="787d8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="787d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="787d8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="787d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="787d8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="787d8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="787d8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="787d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="787d8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="787d8-113">Not supported.</span></span>    |
|<span data-ttu-id="787d8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="787d8-114">Application</span></span> | <span data-ttu-id="787d8-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="787d8-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="787d8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="787d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="787d8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="787d8-117">Request headers</span></span>
| <span data-ttu-id="787d8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="787d8-118">Name</span></span>       | <span data-ttu-id="787d8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="787d8-119">Type</span></span> | <span data-ttu-id="787d8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="787d8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="787d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="787d8-121">Authorization</span></span>  | <span data-ttu-id="787d8-122">string</span><span class="sxs-lookup"><span data-stu-id="787d8-122">string</span></span>  | <span data-ttu-id="787d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="787d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="787d8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="787d8-125">Request body</span></span>
<span data-ttu-id="787d8-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="787d8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="787d8-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="787d8-127">Parameter</span></span>    | <span data-ttu-id="787d8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="787d8-128">Type</span></span>   |<span data-ttu-id="787d8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="787d8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="787d8-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="787d8-130">groupIds</span></span>|<span data-ttu-id="787d8-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="787d8-131">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="787d8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="787d8-132">Response</span></span>

<span data-ttu-id="787d8-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="787d8-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="787d8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="787d8-134">Example</span></span>
<span data-ttu-id="787d8-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="787d8-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="787d8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="787d8-136">Request</span></span>
<span data-ttu-id="787d8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="787d8-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="787d8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="787d8-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="787d8-139">C#</span><span class="sxs-lookup"><span data-stu-id="787d8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="787d8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="787d8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="787d8-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="787d8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="787d8-142">Java</span><span class="sxs-lookup"><span data-stu-id="787d8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="787d8-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="787d8-143">Response</span></span>
<span data-ttu-id="787d8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="787d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
