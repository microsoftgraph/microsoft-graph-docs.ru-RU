---
title: 'orgContact: getMemberObjects'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 02d59a15f4b421c5a49bed8d43638edf5a4d1077
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657247"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="dae86-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="dae86-104">orgContact: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="dae86-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dae86-105">Permissions</span></span>
<span data-ttu-id="dae86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae86-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dae86-108">Permission type</span></span>      | <span data-ttu-id="dae86-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dae86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dae86-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dae86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dae86-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dae86-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dae86-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dae86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dae86-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dae86-113">Not supported.</span></span>    |
|<span data-ttu-id="dae86-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dae86-114">Application</span></span> | <span data-ttu-id="dae86-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae86-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae86-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dae86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="dae86-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dae86-117">Request headers</span></span>
| <span data-ttu-id="dae86-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dae86-118">Name</span></span>       | <span data-ttu-id="dae86-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dae86-119">Type</span></span> | <span data-ttu-id="dae86-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dae86-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dae86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae86-121">Authorization</span></span>  | <span data-ttu-id="dae86-122">string</span><span class="sxs-lookup"><span data-stu-id="dae86-122">string</span></span>  | <span data-ttu-id="dae86-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dae86-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dae86-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dae86-125">Request body</span></span>
<span data-ttu-id="dae86-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dae86-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dae86-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="dae86-127">Parameter</span></span>    | <span data-ttu-id="dae86-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dae86-128">Type</span></span>   |<span data-ttu-id="dae86-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dae86-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dae86-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dae86-130">securityEnabledOnly</span></span>|<span data-ttu-id="dae86-131">Логическое</span><span class="sxs-lookup"><span data-stu-id="dae86-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="dae86-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae86-132">Response</span></span>

<span data-ttu-id="dae86-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dae86-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae86-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dae86-134">Example</span></span>
<span data-ttu-id="dae86-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dae86-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dae86-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="dae86-136">Request</span></span>
<span data-ttu-id="dae86-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dae86-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="dae86-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae86-138">Response</span></span>
<span data-ttu-id="dae86-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dae86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dae86-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dae86-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dae86-143">C#</span><span class="sxs-lookup"><span data-stu-id="dae86-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dae86-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="dae86-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_getmemberobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
