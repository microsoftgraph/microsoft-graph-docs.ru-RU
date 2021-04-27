---
title: Получение entitlementManagementSettings
description: Получение свойств объекта entitlementManagementSettings.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 398a0f75fd4cbf606cbc5c54c509ade4191fb9f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042627"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="e541e-103">Получение entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e541e-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="e541e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e541e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e541e-105">Получение свойств объекта [entitlementManagementSettings.](../resources/entitlementManagementSettings.md)</span><span class="sxs-lookup"><span data-stu-id="e541e-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e541e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e541e-106">Permissions</span></span>

<span data-ttu-id="e541e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e541e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e541e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e541e-109">Permission type</span></span>                        | <span data-ttu-id="e541e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e541e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e541e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e541e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e541e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e541e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e541e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e541e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e541e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e541e-114">Not supported.</span></span> |
| <span data-ttu-id="e541e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e541e-115">Application</span></span>                            | <span data-ttu-id="e541e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e541e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e541e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e541e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e541e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e541e-118">Optional query parameters</span></span>

<span data-ttu-id="e541e-119">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e541e-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e541e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e541e-120">Request headers</span></span>

| <span data-ttu-id="e541e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e541e-121">Name</span></span>      |<span data-ttu-id="e541e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e541e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e541e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e541e-123">Authorization</span></span> | <span data-ttu-id="e541e-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e541e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e541e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e541e-126">Request body</span></span>

<span data-ttu-id="e541e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e541e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e541e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e541e-128">Response</span></span>

<span data-ttu-id="e541e-129">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [entitlementManagementSettings](../resources/entitlementManagementSettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e541e-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e541e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e541e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e541e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e541e-131">Request</span></span>

<span data-ttu-id="e541e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e541e-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e541e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e541e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="e541e-134">C#</span><span class="sxs-lookup"><span data-stu-id="e541e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e541e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e541e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e541e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e541e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e541e-137">Java</span><span class="sxs-lookup"><span data-stu-id="e541e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e541e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e541e-138">Response</span></span>

<span data-ttu-id="e541e-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e541e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e541e-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e541e-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "externalUserLifecycleAction": "None",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


