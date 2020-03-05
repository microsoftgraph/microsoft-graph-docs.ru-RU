---
title: 'servicePrincipal: List oAuth2Permissiongrants'
description: Получение списка объектов oAuth2Permissiongrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9391c0c8d311972a47b57e33d90b4592b275d407
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453398"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="84720-103">servicePrincipal: List oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="84720-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

<span data-ttu-id="84720-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84720-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84720-105">Получение списка объектов oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="84720-105">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="84720-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84720-106">Permissions</span></span>
<span data-ttu-id="84720-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84720-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84720-109">Permission type</span></span>      | <span data-ttu-id="84720-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84720-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84720-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84720-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84720-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84720-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84720-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84720-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84720-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84720-114">Not supported.</span></span>    |
|<span data-ttu-id="84720-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84720-115">Application</span></span> | <span data-ttu-id="84720-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84720-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84720-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84720-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84720-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84720-118">Optional query parameters</span></span>
<span data-ttu-id="84720-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84720-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84720-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84720-120">Request headers</span></span>
| <span data-ttu-id="84720-121">Имя</span><span class="sxs-lookup"><span data-stu-id="84720-121">Name</span></span>       | <span data-ttu-id="84720-122">Тип</span><span class="sxs-lookup"><span data-stu-id="84720-122">Type</span></span> | <span data-ttu-id="84720-123">Описание</span><span class="sxs-lookup"><span data-stu-id="84720-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84720-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84720-124">Authorization</span></span>  | <span data-ttu-id="84720-125">string</span><span class="sxs-lookup"><span data-stu-id="84720-125">string</span></span>  | <span data-ttu-id="84720-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84720-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84720-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84720-128">Request body</span></span>
<span data-ttu-id="84720-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84720-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84720-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="84720-130">Response</span></span>

<span data-ttu-id="84720-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84720-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84720-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84720-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84720-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84720-133">Request</span></span>
<span data-ttu-id="84720-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84720-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84720-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="84720-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
# <a name="c"></a>[<span data-ttu-id="84720-136">C#</span><span class="sxs-lookup"><span data-stu-id="84720-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84720-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84720-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84720-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84720-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84720-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="84720-139">Response</span></span>
<span data-ttu-id="84720-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84720-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
