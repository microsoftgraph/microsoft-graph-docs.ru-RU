---
title: 'servicePrincipal: checkMemberGroups'
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный субъект-служба состоит напрямую или транзитивно.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6f530bf1f5bdb4a7bbb8353aa09471ed708b050b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051979"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="fc696-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fc696-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="fc696-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc696-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc696-106">Проверка участия в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="fc696-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="fc696-107">Возвращает из списка те группы, в которых [servicePrincipal](../resources/serviceprincipal.md) является прямым или транзитивным участниом.</span><span class="sxs-lookup"><span data-stu-id="fc696-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc696-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc696-108">Permissions</span></span>
<span data-ttu-id="fc696-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc696-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc696-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc696-111">Permission type</span></span>      | <span data-ttu-id="fc696-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc696-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc696-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc696-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fc696-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc696-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc696-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc696-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc696-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc696-116">Not supported.</span></span>    |
|<span data-ttu-id="fc696-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc696-117">Application</span></span> | <span data-ttu-id="fc696-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc696-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc696-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc696-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="fc696-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc696-120">Request headers</span></span>
| <span data-ttu-id="fc696-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fc696-121">Name</span></span>       | <span data-ttu-id="fc696-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc696-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="fc696-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc696-123">Authorization</span></span> | <span data-ttu-id="fc696-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc696-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc696-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc696-126">Content-type</span></span> | <span data-ttu-id="fc696-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc696-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc696-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc696-129">Request body</span></span>
<span data-ttu-id="fc696-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc696-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc696-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc696-131">Parameter</span></span>    | <span data-ttu-id="fc696-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fc696-132">Type</span></span>   |<span data-ttu-id="fc696-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fc696-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc696-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="fc696-134">groupIds</span></span>|<span data-ttu-id="fc696-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc696-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="fc696-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc696-136">Response</span></span>

<span data-ttu-id="fc696-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc696-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc696-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc696-138">Examples</span></span>
<span data-ttu-id="fc696-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc696-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="fc696-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc696-140">Request</span></span>
<span data-ttu-id="fc696-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc696-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc696-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc696-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fc696-143">C#</span><span class="sxs-lookup"><span data-stu-id="fc696-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc696-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc696-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc696-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc696-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc696-146">Java</span><span class="sxs-lookup"><span data-stu-id="fc696-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fc696-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc696-147">Response</span></span>
<span data-ttu-id="fc696-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc696-148">Here is an example of the response.</span></span> 
><span data-ttu-id="fc696-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc696-149">Note: The response object shown here might be shortened for readability.</span></span>
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



