---
title: Создание accessPackageCatalog
description: Создание нового accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a9a1190c09cff042783284205def04de3ec4e700
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048549"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="997ee-103">Создание accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="997ee-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="997ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="997ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="997ee-105">Создайте новый [объект accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="997ee-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="997ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="997ee-106">Permissions</span></span>

<span data-ttu-id="997ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="997ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="997ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="997ee-109">Permission type</span></span>                        | <span data-ttu-id="997ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="997ee-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="997ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="997ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="997ee-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997ee-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="997ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="997ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="997ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="997ee-114">Not supported.</span></span> |
| <span data-ttu-id="997ee-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="997ee-115">Application</span></span>                            | <span data-ttu-id="997ee-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997ee-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="997ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="997ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="997ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="997ee-118">Request headers</span></span>

| <span data-ttu-id="997ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="997ee-119">Name</span></span>          | <span data-ttu-id="997ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="997ee-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="997ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="997ee-121">Authorization</span></span> | <span data-ttu-id="997ee-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="997ee-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="997ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="997ee-124">Content-Type</span></span>  | <span data-ttu-id="997ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="997ee-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="997ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="997ee-126">Request body</span></span>

<span data-ttu-id="997ee-127">В теле запроса поставляем представление JSON объекта [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="997ee-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="997ee-128">**Включай имя отображения,** **описание** и **свойства isExternallyVisible.**</span><span class="sxs-lookup"><span data-stu-id="997ee-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="997ee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="997ee-129">Response</span></span>

<span data-ttu-id="997ee-130">В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект accessPackageCatalog](../resources/accesspackagecatalog.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="997ee-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="997ee-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="997ee-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="997ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="997ee-132">Request</span></span>

<span data-ttu-id="997ee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="997ee-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="997ee-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="997ee-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="997ee-135">C#</span><span class="sxs-lookup"><span data-stu-id="997ee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="997ee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="997ee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="997ee-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="997ee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="997ee-138">Java</span><span class="sxs-lookup"><span data-stu-id="997ee-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackagecatalog-from-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="997ee-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="997ee-139">Response</span></span>

<span data-ttu-id="997ee-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="997ee-140">The following is an example of the response.</span></span>

> <span data-ttu-id="997ee-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="997ee-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


