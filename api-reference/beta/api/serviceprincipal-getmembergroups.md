---
title: 'servicePrincipal: getMemberGroups'
description: Список групп, в которых участвует субъект-служба.  Это транзитивная проверка.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d9fd21012f4fe799b18ab07b85683b46ec012c8e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219104"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="cfb40-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="cfb40-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="cfb40-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfb40-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfb40-106">Список групп, в которых участвует субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="cfb40-106">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="cfb40-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="cfb40-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfb40-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfb40-108">Permissions</span></span>
<span data-ttu-id="cfb40-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfb40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cfb40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfb40-111">Permission type</span></span>      | <span data-ttu-id="cfb40-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfb40-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfb40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfb40-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cfb40-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfb40-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfb40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfb40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfb40-116">Not supported.</span></span>    |
|<span data-ttu-id="cfb40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfb40-117">Application</span></span> | <span data-ttu-id="cfb40-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfb40-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfb40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfb40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="cfb40-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfb40-120">Request headers</span></span>
| <span data-ttu-id="cfb40-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cfb40-121">Name</span></span>       | <span data-ttu-id="cfb40-122">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb40-122">Type</span></span> | <span data-ttu-id="cfb40-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb40-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfb40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfb40-124">Authorization</span></span>  | <span data-ttu-id="cfb40-125">string</span><span class="sxs-lookup"><span data-stu-id="cfb40-125">string</span></span>  | <span data-ttu-id="cfb40-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfb40-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfb40-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfb40-128">Request body</span></span>
<span data-ttu-id="cfb40-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cfb40-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cfb40-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="cfb40-130">Parameter</span></span>    | <span data-ttu-id="cfb40-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb40-131">Type</span></span>   |<span data-ttu-id="cfb40-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb40-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfb40-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="cfb40-133">securityEnabledOnly</span></span>|<span data-ttu-id="cfb40-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="cfb40-134">Boolean</span></span>|<span data-ttu-id="cfb40-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="cfb40-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="cfb40-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfb40-137">Response</span></span>

<span data-ttu-id="cfb40-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfb40-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfb40-139">Пример</span><span class="sxs-lookup"><span data-stu-id="cfb40-139">Example</span></span>
<span data-ttu-id="cfb40-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cfb40-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cfb40-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfb40-141">Request</span></span>
<span data-ttu-id="cfb40-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfb40-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfb40-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb40-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cfb40-144">C#</span><span class="sxs-lookup"><span data-stu-id="cfb40-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfb40-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfb40-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfb40-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfb40-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfb40-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfb40-147">Response</span></span>
<span data-ttu-id="cfb40-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cfb40-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
