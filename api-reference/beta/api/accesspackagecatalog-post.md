---
title: Создание Акцесспаккажекаталог
description: Создание нового Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b973310b9cb442f2b95ba4eafd9a2e76ba33fce
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994228"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="51b6a-103">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="51b6a-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b6a-104">Создание нового объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="51b6a-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b6a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51b6a-105">Permissions</span></span>

<span data-ttu-id="51b6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51b6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51b6a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51b6a-108">Permission type</span></span>                        | <span data-ttu-id="51b6a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51b6a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51b6a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51b6a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="51b6a-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b6a-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="51b6a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51b6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b6a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b6a-113">Not supported.</span></span> |
| <span data-ttu-id="51b6a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51b6a-114">Application</span></span>                            | <span data-ttu-id="51b6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b6a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51b6a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51b6a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="51b6a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51b6a-117">Request headers</span></span>

| <span data-ttu-id="51b6a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="51b6a-118">Name</span></span>          | <span data-ttu-id="51b6a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="51b6a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="51b6a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="51b6a-120">Authorization</span></span> | <span data-ttu-id="51b6a-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="51b6a-121">Bearer \{token\}.</span></span> <span data-ttu-id="51b6a-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="51b6a-122">Required.</span></span> |
| <span data-ttu-id="51b6a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51b6a-123">Content-Type</span></span>  | <span data-ttu-id="51b6a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51b6a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51b6a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51b6a-125">Request body</span></span>

<span data-ttu-id="51b6a-126">В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51b6a-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="51b6a-127">Включите свойства **DisplayName**, **Description**и **исекстерналливисибле** .</span><span class="sxs-lookup"><span data-stu-id="51b6a-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="51b6a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="51b6a-128">Response</span></span>

<span data-ttu-id="51b6a-129">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51b6a-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51b6a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="51b6a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51b6a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="51b6a-131">Request</span></span>

<span data-ttu-id="51b6a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51b6a-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51b6a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="51b6a-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="51b6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="51b6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51b6a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51b6a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51b6a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51b6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51b6a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="51b6a-137">Response</span></span>

<span data-ttu-id="51b6a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51b6a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="51b6a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51b6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
