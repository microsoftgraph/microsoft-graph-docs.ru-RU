---
title: 'servicePrincipal: getMemberGroups'
description: Список групп, в которых участвует субъект-служба.  Это транзитивная проверка.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 40fa4162a5aea180507c0cbc04bbe095de466f3e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453471"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="1a9b2-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1a9b2-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="1a9b2-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a9b2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a9b2-106">Список групп, в которых участвует субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-106">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="1a9b2-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a9b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9b2-108">Permissions</span></span>
<span data-ttu-id="1a9b2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a9b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a9b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9b2-111">Permission type</span></span>      | <span data-ttu-id="1a9b2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a9b2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a9b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a9b2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1a9b2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a9b2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a9b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a9b2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a9b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-116">Not supported.</span></span>    |
|<span data-ttu-id="1a9b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a9b2-117">Application</span></span> | <span data-ttu-id="1a9b2-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a9b2-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a9b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a9b2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="1a9b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a9b2-120">Request headers</span></span>
| <span data-ttu-id="1a9b2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1a9b2-121">Name</span></span>       | <span data-ttu-id="1a9b2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1a9b2-122">Type</span></span> | <span data-ttu-id="1a9b2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9b2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1a9b2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a9b2-124">Authorization</span></span>  | <span data-ttu-id="1a9b2-125">string</span><span class="sxs-lookup"><span data-stu-id="1a9b2-125">string</span></span>  | <span data-ttu-id="1a9b2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a9b2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a9b2-128">Request body</span></span>
<span data-ttu-id="1a9b2-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a9b2-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a9b2-130">Parameter</span></span>    | <span data-ttu-id="1a9b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a9b2-131">Type</span></span>   |<span data-ttu-id="1a9b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9b2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a9b2-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1a9b2-133">securityEnabledOnly</span></span>|<span data-ttu-id="1a9b2-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="1a9b2-134">Boolean</span></span>|<span data-ttu-id="1a9b2-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="1a9b2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a9b2-137">Response</span></span>

<span data-ttu-id="1a9b2-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a9b2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1a9b2-139">Example</span></span>
<span data-ttu-id="1a9b2-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a9b2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a9b2-141">Request</span></span>
<span data-ttu-id="1a9b2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a9b2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a9b2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="1a9b2-144">C#</span><span class="sxs-lookup"><span data-stu-id="1a9b2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a9b2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a9b2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a9b2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a9b2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1a9b2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a9b2-147">Response</span></span>
<span data-ttu-id="1a9b2-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a9b2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
