---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a373fab5ce1d16f9db0568c4a2dc14fc77d7fdef
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655931"
---
# <a name="list-directoryroles"></a><span data-ttu-id="b3d20-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="b3d20-103">List directoryRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3d20-104">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b3d20-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3d20-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d20-105">Permissions</span></span>
<span data-ttu-id="b3d20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d20-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d20-108">Permission type</span></span>      | <span data-ttu-id="b3d20-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3d20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3d20-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3d20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3d20-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3d20-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3d20-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3d20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d20-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d20-113">Not supported.</span></span>    |
|<span data-ttu-id="b3d20-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3d20-114">Application</span></span> | <span data-ttu-id="b3d20-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d20-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d20-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3d20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3d20-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3d20-117">Optional query parameters</span></span>
<span data-ttu-id="b3d20-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="b3d20-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3d20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3d20-119">Request headers</span></span>
| <span data-ttu-id="b3d20-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b3d20-120">Name</span></span>       | <span data-ttu-id="b3d20-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b3d20-121">Type</span></span> | <span data-ttu-id="b3d20-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d20-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3d20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d20-123">Authorization</span></span>  | <span data-ttu-id="b3d20-124">string</span><span class="sxs-lookup"><span data-stu-id="b3d20-124">string</span></span>  | <span data-ttu-id="b3d20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3d20-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3d20-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3d20-127">Request body</span></span>
<span data-ttu-id="b3d20-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3d20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3d20-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3d20-129">Response</span></span>

<span data-ttu-id="b3d20-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3d20-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3d20-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b3d20-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3d20-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3d20-132">Request</span></span>
<span data-ttu-id="b3d20-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3d20-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="b3d20-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d20-134">Response</span></span>
<span data-ttu-id="b3d20-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3d20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b3d20-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b3d20-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b3d20-139">C#</span><span class="sxs-lookup"><span data-stu-id="b3d20-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3d20-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3d20-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryroles-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
