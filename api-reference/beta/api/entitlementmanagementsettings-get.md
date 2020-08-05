---
title: Получение Ентитлементманажементсеттингс
description: Получение свойств объекта Ентитлементманажементсеттингс.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5a0e77a41ef3517eb55ab9669ab994f871024e1
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566903"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="96de8-103">Получение Ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="96de8-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="96de8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96de8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96de8-105">Получение свойств объекта [ентитлементманажементсеттингс](../resources/entitlementManagementSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="96de8-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96de8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96de8-106">Permissions</span></span>

<span data-ttu-id="96de8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96de8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96de8-109">Permission type</span></span>                        | <span data-ttu-id="96de8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96de8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96de8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96de8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96de8-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="96de8-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="96de8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96de8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96de8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96de8-114">Not supported.</span></span> |
| <span data-ttu-id="96de8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96de8-115">Application</span></span>                            | <span data-ttu-id="96de8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96de8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96de8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96de8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96de8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96de8-118">Optional query parameters</span></span>

<span data-ttu-id="96de8-119">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="96de8-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96de8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96de8-120">Request headers</span></span>

| <span data-ttu-id="96de8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="96de8-121">Name</span></span>      |<span data-ttu-id="96de8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="96de8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96de8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96de8-123">Authorization</span></span> | <span data-ttu-id="96de8-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="96de8-124">Bearer \{token\}.</span></span> <span data-ttu-id="96de8-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="96de8-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96de8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96de8-126">Request body</span></span>

<span data-ttu-id="96de8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96de8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96de8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="96de8-128">Response</span></span>

<span data-ttu-id="96de8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [ентитлементманажементсеттингс](../resources/entitlementManagementSettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96de8-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96de8-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="96de8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96de8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="96de8-131">Request</span></span>

<span data-ttu-id="96de8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96de8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96de8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="96de8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="96de8-134">C#</span><span class="sxs-lookup"><span data-stu-id="96de8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96de8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96de8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96de8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96de8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="96de8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="96de8-137">Response</span></span>

<span data-ttu-id="96de8-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96de8-138">The following is an example of the response.</span></span>

> <span data-ttu-id="96de8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96de8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
