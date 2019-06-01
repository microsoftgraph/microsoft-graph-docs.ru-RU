---
title: Получение directoryRole
description: Получение свойств объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aba5f7fc9773e9f8e49e1346ecadbd690c62c0a2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655959"
---
# <a name="get-directoryrole"></a><span data-ttu-id="fdd63-103">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="fdd63-103">Get directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd63-104">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="fdd63-104">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdd63-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd63-105">Permissions</span></span>
<span data-ttu-id="fdd63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdd63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd63-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd63-108">Permission type</span></span>      | <span data-ttu-id="fdd63-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdd63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdd63-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdd63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fdd63-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fdd63-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fdd63-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdd63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdd63-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd63-113">Not supported.</span></span>    |
|<span data-ttu-id="fdd63-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdd63-114">Application</span></span> | <span data-ttu-id="fdd63-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd63-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdd63-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdd63-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fdd63-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fdd63-117">Optional query parameters</span></span>
<span data-ttu-id="fdd63-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="fdd63-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdd63-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdd63-119">Request headers</span></span>
| <span data-ttu-id="fdd63-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fdd63-120">Name</span></span>       | <span data-ttu-id="fdd63-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fdd63-121">Type</span></span> | <span data-ttu-id="fdd63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fdd63-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fdd63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdd63-123">Authorization</span></span>  | <span data-ttu-id="fdd63-124">string</span><span class="sxs-lookup"><span data-stu-id="fdd63-124">string</span></span>  | <span data-ttu-id="fdd63-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdd63-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdd63-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdd63-127">Request body</span></span>
<span data-ttu-id="fdd63-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdd63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdd63-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdd63-129">Response</span></span>

<span data-ttu-id="fdd63-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdd63-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fdd63-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fdd63-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdd63-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdd63-132">Request</span></span>
<span data-ttu-id="fdd63-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdd63-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="fdd63-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd63-134">Response</span></span>
<span data-ttu-id="fdd63-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdd63-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fdd63-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fdd63-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fdd63-139">C#</span><span class="sxs-lookup"><span data-stu-id="fdd63-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdd63-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdd63-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
