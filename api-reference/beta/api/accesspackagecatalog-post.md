---
title: Создание accessPackageCatalog
description: Создание нового accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 783744f3e2cfc59f20e2105468b5f2cdc2d7ee7d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439529"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="a60a6-103">Создание accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a60a6-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="a60a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a60a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a60a6-105">Создайте новый [объект accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="a60a6-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a60a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a60a6-106">Permissions</span></span>

<span data-ttu-id="a60a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a60a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a60a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a60a6-109">Permission type</span></span>                        | <span data-ttu-id="a60a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a60a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a60a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a60a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a60a6-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a60a6-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a60a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a60a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a60a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a60a6-114">Not supported.</span></span> |
| <span data-ttu-id="a60a6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a60a6-115">Application</span></span>                            | <span data-ttu-id="a60a6-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a60a6-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a60a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a60a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="a60a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a60a6-118">Request headers</span></span>

| <span data-ttu-id="a60a6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a60a6-119">Name</span></span>          | <span data-ttu-id="a60a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a60a6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a60a6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a60a6-121">Authorization</span></span> | <span data-ttu-id="a60a6-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a60a6-122">Bearer \{token\}.</span></span> <span data-ttu-id="a60a6-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a60a6-123">Required.</span></span> |
| <span data-ttu-id="a60a6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a60a6-124">Content-Type</span></span>  | <span data-ttu-id="a60a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a60a6-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a60a6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a60a6-126">Request body</span></span>

<span data-ttu-id="a60a6-127">В теле запроса поставляем представление JSON объекта [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="a60a6-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="a60a6-128">**Включай имя отображения,** **описание** и **свойства isExternallyVisible.**</span><span class="sxs-lookup"><span data-stu-id="a60a6-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="a60a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a60a6-129">Response</span></span>

<span data-ttu-id="a60a6-130">В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект accessPackageCatalog](../resources/accesspackagecatalog.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a60a6-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a60a6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a60a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a60a6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a60a6-132">Request</span></span>

<span data-ttu-id="a60a6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a60a6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a60a6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a60a6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```
# <a name="c"></a>[<span data-ttu-id="a60a6-135">C#</span><span class="sxs-lookup"><span data-stu-id="a60a6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a60a6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a60a6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a60a6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a60a6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a60a6-138">Java</span><span class="sxs-lookup"><span data-stu-id="a60a6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackagecatalog-from-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a60a6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a60a6-139">Response</span></span>

<span data-ttu-id="a60a6-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a60a6-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a60a6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a60a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


