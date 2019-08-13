---
title: 'servicePrincipal: getMemberObjects'
description: Получение списка групп и ролей каталогов, членом которых является данный участник службы.  Эта проверка является транзитивным.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 13d0939ee61fe4b56b931c4938d75ec553e0eeb4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364042"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="76884-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="76884-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76884-105">Получение списка групп и ролей каталогов, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="76884-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="76884-106">Эта проверка является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="76884-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="76884-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76884-107">Permissions</span></span>
<span data-ttu-id="76884-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76884-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76884-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76884-110">Permission type</span></span>      | <span data-ttu-id="76884-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76884-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76884-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76884-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76884-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76884-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="76884-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76884-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76884-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76884-115">Not supported.</span></span>    |
|<span data-ttu-id="76884-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76884-116">Application</span></span> | <span data-ttu-id="76884-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76884-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76884-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76884-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="76884-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76884-119">Request headers</span></span>
| <span data-ttu-id="76884-120">Имя</span><span class="sxs-lookup"><span data-stu-id="76884-120">Name</span></span>       | <span data-ttu-id="76884-121">Тип</span><span class="sxs-lookup"><span data-stu-id="76884-121">Type</span></span> | <span data-ttu-id="76884-122">Описание</span><span class="sxs-lookup"><span data-stu-id="76884-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76884-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76884-123">Authorization</span></span>  | <span data-ttu-id="76884-124">string</span><span class="sxs-lookup"><span data-stu-id="76884-124">string</span></span>  | <span data-ttu-id="76884-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76884-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76884-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76884-127">Request body</span></span>
<span data-ttu-id="76884-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="76884-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76884-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="76884-129">Parameter</span></span>    | <span data-ttu-id="76884-130">Тип</span><span class="sxs-lookup"><span data-stu-id="76884-130">Type</span></span>   |<span data-ttu-id="76884-131">Описание</span><span class="sxs-lookup"><span data-stu-id="76884-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76884-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="76884-132">securityEnabledOnly</span></span>|<span data-ttu-id="76884-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="76884-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="76884-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="76884-134">Response</span></span>

<span data-ttu-id="76884-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76884-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76884-136">Пример</span><span class="sxs-lookup"><span data-stu-id="76884-136">Example</span></span>
<span data-ttu-id="76884-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="76884-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76884-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="76884-138">Request</span></span>
<span data-ttu-id="76884-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76884-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76884-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="76884-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76884-141">C#</span><span class="sxs-lookup"><span data-stu-id="76884-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76884-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76884-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76884-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="76884-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="76884-144">Java</span><span class="sxs-lookup"><span data-stu-id="76884-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="76884-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="76884-145">Response</span></span>
<span data-ttu-id="76884-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76884-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
