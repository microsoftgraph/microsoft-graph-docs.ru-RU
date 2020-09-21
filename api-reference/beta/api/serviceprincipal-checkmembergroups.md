---
title: 'servicePrincipal: checkMemberGroups'
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых субъект-служба является прямым или транзитивным участником.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2e36d11d63d0ce8cd5ab5a1e8b894d4638c22eaf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044692"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="b3d95-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b3d95-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="b3d95-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3d95-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3d95-106">Проверка участия в указанном списке групп.</span><span class="sxs-lookup"><span data-stu-id="b3d95-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="b3d95-107">Возвращает из списка те группы, в которых [servicePrincipal](../resources/serviceprincipal.md) является прямым или транзитивным участниом.</span><span class="sxs-lookup"><span data-stu-id="b3d95-107">Returns from the list those groups of which the [servicePrincipal](../resources/serviceprincipal.md) has a direct or transitive membership.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d95-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d95-108">Permissions</span></span>
<span data-ttu-id="b3d95-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d95-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d95-111">Permission type</span></span>      | <span data-ttu-id="b3d95-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3d95-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3d95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3d95-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3d95-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3d95-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3d95-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3d95-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d95-116">Not supported.</span></span>    |
|<span data-ttu-id="b3d95-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3d95-117">Application</span></span> | <span data-ttu-id="b3d95-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d95-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d95-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3d95-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="b3d95-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3d95-120">Request headers</span></span>
| <span data-ttu-id="b3d95-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b3d95-121">Name</span></span>       | <span data-ttu-id="b3d95-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d95-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="b3d95-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3d95-123">Authorization</span></span> | <span data-ttu-id="b3d95-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3d95-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3d95-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3d95-126">Content-type</span></span> | <span data-ttu-id="b3d95-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3d95-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3d95-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3d95-129">Request body</span></span>
<span data-ttu-id="b3d95-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b3d95-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3d95-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3d95-131">Parameter</span></span>    | <span data-ttu-id="b3d95-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b3d95-132">Type</span></span>   |<span data-ttu-id="b3d95-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d95-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3d95-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="b3d95-134">groupIds</span></span>|<span data-ttu-id="b3d95-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3d95-135">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="b3d95-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d95-136">Response</span></span>

<span data-ttu-id="b3d95-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3d95-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3d95-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3d95-138">Examples</span></span>
<span data-ttu-id="b3d95-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b3d95-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="b3d95-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3d95-140">Request</span></span>
<span data-ttu-id="b3d95-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3d95-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3d95-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3d95-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b3d95-143">C#</span><span class="sxs-lookup"><span data-stu-id="b3d95-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3d95-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3d95-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3d95-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3d95-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b3d95-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d95-146">Response</span></span>
<span data-ttu-id="b3d95-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3d95-147">Here is an example of the response.</span></span> 
><span data-ttu-id="b3d95-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3d95-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


