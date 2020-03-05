---
title: Создание Акцесспаккажекаталог
description: Создание нового Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90a340de45fc0f31e1b5bd534151c449a2b315af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441965"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="90a44-103">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="90a44-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="90a44-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90a44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a44-105">Создание нового объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="90a44-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90a44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90a44-106">Permissions</span></span>

<span data-ttu-id="90a44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90a44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90a44-109">Permission type</span></span>                        | <span data-ttu-id="90a44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90a44-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90a44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90a44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90a44-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90a44-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="90a44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90a44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90a44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a44-114">Not supported.</span></span> |
| <span data-ttu-id="90a44-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90a44-115">Application</span></span>                            | <span data-ttu-id="90a44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a44-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90a44-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90a44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="90a44-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90a44-118">Request headers</span></span>

| <span data-ttu-id="90a44-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90a44-119">Name</span></span>          | <span data-ttu-id="90a44-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90a44-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90a44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90a44-121">Authorization</span></span> | <span data-ttu-id="90a44-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="90a44-122">Bearer \{token\}.</span></span> <span data-ttu-id="90a44-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="90a44-123">Required.</span></span> |
| <span data-ttu-id="90a44-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90a44-124">Content-Type</span></span>  | <span data-ttu-id="90a44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90a44-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90a44-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90a44-126">Request body</span></span>

<span data-ttu-id="90a44-127">В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90a44-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="90a44-128">Включите свойства **DisplayName**, **Description**и **исекстерналливисибле** .</span><span class="sxs-lookup"><span data-stu-id="90a44-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="90a44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90a44-129">Response</span></span>

<span data-ttu-id="90a44-130">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90a44-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90a44-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="90a44-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90a44-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90a44-132">Request</span></span>

<span data-ttu-id="90a44-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90a44-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90a44-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90a44-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="90a44-135">C#</span><span class="sxs-lookup"><span data-stu-id="90a44-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90a44-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90a44-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90a44-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90a44-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90a44-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90a44-138">Response</span></span>

<span data-ttu-id="90a44-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90a44-139">The following is an example of the response.</span></span>

> <span data-ttu-id="90a44-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90a44-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
