---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf36b48d2f0a1aa5478a78ad211348a815e0d790
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456623"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="98dbc-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="98dbc-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="98dbc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98dbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98dbc-105">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="98dbc-105">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="98dbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98dbc-106">Permissions</span></span>

<span data-ttu-id="98dbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98dbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="98dbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98dbc-109">Permission type</span></span>      | <span data-ttu-id="98dbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98dbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98dbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98dbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98dbc-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="98dbc-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98dbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98dbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98dbc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98dbc-114">Not supported.</span></span>    |
|<span data-ttu-id="98dbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98dbc-115">Application</span></span> | <span data-ttu-id="98dbc-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98dbc-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98dbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98dbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98dbc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98dbc-118">Optional query parameters</span></span>
<span data-ttu-id="98dbc-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98dbc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98dbc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98dbc-120">Request headers</span></span>
| <span data-ttu-id="98dbc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="98dbc-121">Name</span></span> | <span data-ttu-id="98dbc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="98dbc-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="98dbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98dbc-123">Authorization</span></span>  | <span data-ttu-id="98dbc-124">string</span><span class="sxs-lookup"><span data-stu-id="98dbc-124">string</span></span>  | <span data-ttu-id="98dbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98dbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98dbc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98dbc-127">Request body</span></span>
<span data-ttu-id="98dbc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98dbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98dbc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="98dbc-129">Response</span></span>

<span data-ttu-id="98dbc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98dbc-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98dbc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98dbc-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98dbc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98dbc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98dbc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="98dbc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="98dbc-134">C#</span><span class="sxs-lookup"><span data-stu-id="98dbc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98dbc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98dbc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98dbc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98dbc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98dbc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="98dbc-137">Response</span></span>

<span data-ttu-id="98dbc-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98dbc-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
