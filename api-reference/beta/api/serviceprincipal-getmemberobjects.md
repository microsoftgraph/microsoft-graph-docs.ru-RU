---
title: 'servicePrincipal: getMemberObjects'
description: Список групп и ролей каталога, в которых участвует субъект-служба.  Эта проверка является транзитивным.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: afa2e48691ba421fad8ffc1c2f5ae630591295d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453459"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="070f7-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="070f7-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="070f7-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="070f7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="070f7-106">Список групп и ролей каталога, в которых участвует субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="070f7-106">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="070f7-107">Эта проверка является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="070f7-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="070f7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="070f7-108">Permissions</span></span>
<span data-ttu-id="070f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="070f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="070f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="070f7-111">Permission type</span></span>      | <span data-ttu-id="070f7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="070f7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="070f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="070f7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="070f7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="070f7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="070f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="070f7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="070f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="070f7-116">Not supported.</span></span>    |
|<span data-ttu-id="070f7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="070f7-117">Application</span></span> | <span data-ttu-id="070f7-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="070f7-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="070f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="070f7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="070f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="070f7-120">Request headers</span></span>
| <span data-ttu-id="070f7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="070f7-121">Name</span></span>       | <span data-ttu-id="070f7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="070f7-122">Type</span></span> | <span data-ttu-id="070f7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="070f7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="070f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="070f7-124">Authorization</span></span>  | <span data-ttu-id="070f7-125">string</span><span class="sxs-lookup"><span data-stu-id="070f7-125">string</span></span>  | <span data-ttu-id="070f7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="070f7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="070f7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="070f7-128">Request body</span></span>
<span data-ttu-id="070f7-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="070f7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="070f7-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="070f7-130">Parameter</span></span>    | <span data-ttu-id="070f7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="070f7-131">Type</span></span>   |<span data-ttu-id="070f7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="070f7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="070f7-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="070f7-133">securityEnabledOnly</span></span>|<span data-ttu-id="070f7-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="070f7-134">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="070f7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="070f7-135">Response</span></span>

<span data-ttu-id="070f7-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="070f7-136">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="070f7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="070f7-137">Example</span></span>
<span data-ttu-id="070f7-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="070f7-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="070f7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="070f7-139">Request</span></span>
<span data-ttu-id="070f7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="070f7-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="070f7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="070f7-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="070f7-142">C#</span><span class="sxs-lookup"><span data-stu-id="070f7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="070f7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="070f7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="070f7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="070f7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="070f7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="070f7-145">Response</span></span>
<span data-ttu-id="070f7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="070f7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
