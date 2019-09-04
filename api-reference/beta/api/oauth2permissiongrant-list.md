---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 84dc12fc863dafa8602e99332cf152c217dc23e1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723863"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="dd347-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="dd347-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd347-104">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="dd347-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd347-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd347-105">Permissions</span></span>

<span data-ttu-id="dd347-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd347-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd347-108">Permission type</span></span>      | <span data-ttu-id="dd347-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd347-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd347-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd347-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd347-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd347-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd347-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd347-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd347-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd347-113">Not supported.</span></span>    |
|<span data-ttu-id="dd347-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd347-114">Application</span></span> | <span data-ttu-id="dd347-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd347-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd347-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd347-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd347-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd347-117">Optional query parameters</span></span>
<span data-ttu-id="dd347-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd347-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd347-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd347-119">Request headers</span></span>
| <span data-ttu-id="dd347-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dd347-120">Name</span></span> | <span data-ttu-id="dd347-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dd347-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="dd347-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd347-122">Authorization</span></span>  | <span data-ttu-id="dd347-123">string</span><span class="sxs-lookup"><span data-stu-id="dd347-123">string</span></span>  | <span data-ttu-id="dd347-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd347-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd347-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd347-126">Request body</span></span>
<span data-ttu-id="dd347-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd347-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd347-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd347-128">Response</span></span>

<span data-ttu-id="dd347-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd347-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd347-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dd347-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd347-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd347-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd347-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd347-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd347-133">C#</span><span class="sxs-lookup"><span data-stu-id="dd347-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd347-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd347-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd347-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dd347-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd347-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd347-136">Response</span></span>

<span data-ttu-id="dd347-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd347-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
