---
title: 'orgContact: Чеккмемберграупс'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 057d2a76d18db261b7ff1a4de238a3fe7006839a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657282"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="a849d-104">orgContact: Чеккмемберграупс</span><span class="sxs-lookup"><span data-stu-id="a849d-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="a849d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a849d-105">Permissions</span></span>
<span data-ttu-id="a849d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a849d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a849d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a849d-108">Permission type</span></span>      | <span data-ttu-id="a849d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a849d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a849d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a849d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a849d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a849d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a849d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a849d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a849d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a849d-113">Not supported.</span></span>    |
|<span data-ttu-id="a849d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a849d-114">Application</span></span> | <span data-ttu-id="a849d-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a849d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a849d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a849d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="a849d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a849d-117">Request headers</span></span>
| <span data-ttu-id="a849d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a849d-118">Name</span></span>       | <span data-ttu-id="a849d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a849d-119">Type</span></span> | <span data-ttu-id="a849d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a849d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a849d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a849d-121">Authorization</span></span>  | <span data-ttu-id="a849d-122">string</span><span class="sxs-lookup"><span data-stu-id="a849d-122">string</span></span>  | <span data-ttu-id="a849d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a849d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a849d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a849d-125">Request body</span></span>
<span data-ttu-id="a849d-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a849d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a849d-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="a849d-127">Parameter</span></span>    | <span data-ttu-id="a849d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a849d-128">Type</span></span>   |<span data-ttu-id="a849d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a849d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a849d-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="a849d-130">groupIds</span></span>|<span data-ttu-id="a849d-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a849d-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="a849d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a849d-132">Response</span></span>

<span data-ttu-id="a849d-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a849d-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a849d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a849d-134">Example</span></span>
<span data-ttu-id="a849d-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a849d-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a849d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a849d-136">Request</span></span>
<span data-ttu-id="a849d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a849d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="a849d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a849d-138">Response</span></span>
<span data-ttu-id="a849d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a849d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a849d-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a849d-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a849d-143">C#</span><span class="sxs-lookup"><span data-stu-id="a849d-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a849d-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="a849d-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
