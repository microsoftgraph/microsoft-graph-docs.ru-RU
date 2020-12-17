---
title: 'servicePrincipal: checkMemberGroups'
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых субъект-служба является прямым или транзитивным участником.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: a443719d1792e3abc0540b2ea8b26140a48a5af8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970906"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="e6f54-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e6f54-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="e6f54-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f54-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f54-106">Проверка участия в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="e6f54-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="e6f54-107">Возвращает из списка те группы, в которых [servicePrincipal](../resources/serviceprincipal.md) является прямым или транзитивным участниом.</span><span class="sxs-lookup"><span data-stu-id="e6f54-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f54-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f54-108">Permissions</span></span>
<span data-ttu-id="e6f54-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f54-111">Permission type</span></span>      | <span data-ttu-id="e6f54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6f54-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6f54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6f54-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e6f54-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6f54-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6f54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6f54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f54-116">Not supported.</span></span>    |
|<span data-ttu-id="e6f54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6f54-117">Application</span></span> | <span data-ttu-id="e6f54-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f54-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6f54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6f54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e6f54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6f54-120">Request headers</span></span>
| <span data-ttu-id="e6f54-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e6f54-121">Name</span></span>       | <span data-ttu-id="e6f54-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e6f54-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e6f54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6f54-123">Authorization</span></span> | <span data-ttu-id="e6f54-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6f54-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e6f54-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6f54-126">Content-type</span></span> | <span data-ttu-id="e6f54-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6f54-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6f54-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6f54-129">Request body</span></span>
<span data-ttu-id="e6f54-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e6f54-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6f54-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e6f54-131">Parameter</span></span>    | <span data-ttu-id="e6f54-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e6f54-132">Type</span></span>   |<span data-ttu-id="e6f54-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e6f54-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f54-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="e6f54-134">groupIds</span></span>|<span data-ttu-id="e6f54-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e6f54-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="e6f54-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f54-136">Response</span></span>

<span data-ttu-id="e6f54-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6f54-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6f54-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="e6f54-138">Examples</span></span>
<span data-ttu-id="e6f54-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e6f54-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="e6f54-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6f54-140">Request</span></span>
<span data-ttu-id="e6f54-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6f54-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6f54-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f54-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6f54-143">C#</span><span class="sxs-lookup"><span data-stu-id="e6f54-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6f54-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6f54-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6f54-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6f54-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6f54-146">Java</span><span class="sxs-lookup"><span data-stu-id="e6f54-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e6f54-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f54-147">Response</span></span>
<span data-ttu-id="e6f54-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6f54-148">Here is an example of the response.</span></span> 
><span data-ttu-id="e6f54-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6f54-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


