---
title: Получение directoryRole
description: Получение свойств объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 543b5187a79aa00479ffd6e8a3f1178038a05884
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278983"
---
# <a name="get-directoryrole"></a><span data-ttu-id="f711a-103">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="f711a-103">Get directoryRole</span></span>

<span data-ttu-id="f711a-104">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="f711a-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f711a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f711a-105">Permissions</span></span>
<span data-ttu-id="f711a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f711a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f711a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f711a-108">Permission type</span></span>      | <span data-ttu-id="f711a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f711a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f711a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f711a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f711a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f711a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f711a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f711a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f711a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f711a-113">Not supported.</span></span>    |
|<span data-ttu-id="f711a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f711a-114">Application</span></span> | <span data-ttu-id="f711a-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f711a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f711a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f711a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f711a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f711a-117">Optional query parameters</span></span>
<span data-ttu-id="f711a-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="f711a-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f711a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f711a-119">Request headers</span></span>
| <span data-ttu-id="f711a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f711a-120">Name</span></span>       | <span data-ttu-id="f711a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f711a-121">Type</span></span> | <span data-ttu-id="f711a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f711a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f711a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f711a-123">Authorization</span></span>  | <span data-ttu-id="f711a-124">string</span><span class="sxs-lookup"><span data-stu-id="f711a-124">string</span></span>  | <span data-ttu-id="f711a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f711a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f711a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f711a-127">Request body</span></span>
<span data-ttu-id="f711a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f711a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f711a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f711a-129">Response</span></span>

<span data-ttu-id="f711a-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f711a-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f711a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f711a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f711a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f711a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="f711a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f711a-133">Response</span></span>
<span data-ttu-id="f711a-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f711a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f711a-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f711a-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f711a-137">C#</span><span class="sxs-lookup"><span data-stu-id="f711a-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f711a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f711a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f711a-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f711a-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryrole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
