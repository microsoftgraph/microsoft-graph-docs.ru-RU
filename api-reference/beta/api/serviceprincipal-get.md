---
title: Получение объекта servicePrincipal
description: Получение свойств и связей объекта serviceprincipal.
localization_priority: Priority
ms.openlocfilehash: 9f28a2e2da61b852422ee8efd453cc5d98f910be
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638748"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="46223-103">Получение объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="46223-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46223-104">Получение свойств и связей объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="46223-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46223-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46223-105">Permissions</span></span>
<span data-ttu-id="46223-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="46223-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46223-108">Permission type</span></span>      | <span data-ttu-id="46223-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46223-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46223-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46223-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46223-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46223-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46223-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46223-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46223-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46223-113">Not supported.</span></span>    |
|<span data-ttu-id="46223-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46223-114">Application</span></span> | <span data-ttu-id="46223-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="46223-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46223-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46223-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46223-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46223-117">Optional query parameters</span></span>
<span data-ttu-id="46223-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="46223-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46223-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46223-119">Request headers</span></span>
| <span data-ttu-id="46223-120">Имя</span><span class="sxs-lookup"><span data-stu-id="46223-120">Name</span></span>       | <span data-ttu-id="46223-121">Тип</span><span class="sxs-lookup"><span data-stu-id="46223-121">Type</span></span> | <span data-ttu-id="46223-122">Описание</span><span class="sxs-lookup"><span data-stu-id="46223-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46223-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46223-123">Authorization</span></span>  | <span data-ttu-id="46223-124">string</span><span class="sxs-lookup"><span data-stu-id="46223-124">string</span></span>  | <span data-ttu-id="46223-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46223-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46223-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46223-127">Request body</span></span>
<span data-ttu-id="46223-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46223-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46223-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="46223-129">Response</span></span>

<span data-ttu-id="46223-130">В случае успеха этот метод возвращает код ответа `200 OK` и объект [servicePrincipal](../resources/serviceprincipal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="46223-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46223-131">Пример</span><span class="sxs-lookup"><span data-stu-id="46223-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46223-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46223-132">Request</span></span>
<span data-ttu-id="46223-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46223-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="46223-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="46223-134">Response</span></span>
<span data-ttu-id="46223-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46223-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="46223-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="46223-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="46223-139">C#</span><span class="sxs-lookup"><span data-stu-id="46223-139">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46223-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="46223-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
