---
title: 'servicePrincipal: getMemberGroups'
description: Получение списка групп, членом которых является данный участник службы.  Это транзитивная проверка.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a6f1fce9f5995762c120ad14597834b06d8b07a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410328"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="ecae4-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ecae4-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecae4-105">Получение списка групп, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="ecae4-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="ecae4-106">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ecae4-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecae4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecae4-107">Permissions</span></span>
<span data-ttu-id="ecae4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecae4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ecae4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecae4-110">Permission type</span></span>      | <span data-ttu-id="ecae4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecae4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecae4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecae4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ecae4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ecae4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ecae4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecae4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecae4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecae4-115">Not supported.</span></span>    |
|<span data-ttu-id="ecae4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecae4-116">Application</span></span> | <span data-ttu-id="ecae4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecae4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecae4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecae4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="ecae4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecae4-119">Request headers</span></span>
| <span data-ttu-id="ecae4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ecae4-120">Name</span></span>       | <span data-ttu-id="ecae4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ecae4-121">Type</span></span> | <span data-ttu-id="ecae4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ecae4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ecae4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecae4-123">Authorization</span></span>  | <span data-ttu-id="ecae4-124">string</span><span class="sxs-lookup"><span data-stu-id="ecae4-124">string</span></span>  | <span data-ttu-id="ecae4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecae4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecae4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ecae4-127">Request body</span></span>
<span data-ttu-id="ecae4-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ecae4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ecae4-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="ecae4-129">Parameter</span></span>    | <span data-ttu-id="ecae4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ecae4-130">Type</span></span>   |<span data-ttu-id="ecae4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ecae4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecae4-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ecae4-132">securityEnabledOnly</span></span>|<span data-ttu-id="ecae4-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="ecae4-133">Boolean</span></span>|<span data-ttu-id="ecae4-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="ecae4-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="ecae4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecae4-136">Response</span></span>

<span data-ttu-id="ecae4-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecae4-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecae4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ecae4-138">Example</span></span>
<span data-ttu-id="ecae4-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ecae4-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ecae4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecae4-140">Request</span></span>
<span data-ttu-id="ecae4-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecae4-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ecae4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecae4-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ecae4-143">C#</span><span class="sxs-lookup"><span data-stu-id="ecae4-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecae4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecae4-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ecae4-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ecae4-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ecae4-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecae4-146">Response</span></span>
<span data-ttu-id="ecae4-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecae4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
