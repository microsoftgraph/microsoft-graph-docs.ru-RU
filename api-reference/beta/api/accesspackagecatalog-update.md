---
title: Обновление accessPackageCatalog
description: Обновление свойств объекта accessPackageCatalog.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7bb4b1cadfd3991f19ff02b5ad596f5a8ff1491
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872165"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="40dbe-103">Обновление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="40dbe-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="40dbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40dbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40dbe-105">Обновите [существующий объект accessPackageCatalog,](../resources/accesspackagecatalog.md) чтобы изменить одно или несколько его свойств, например отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="40dbe-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="40dbe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40dbe-106">Permissions</span></span>
<span data-ttu-id="40dbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40dbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="40dbe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40dbe-109">Permission type</span></span>|<span data-ttu-id="40dbe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40dbe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40dbe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40dbe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40dbe-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dbe-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="40dbe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40dbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40dbe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40dbe-114">Not supported.</span></span> |
|<span data-ttu-id="40dbe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40dbe-115">Application</span></span>                            | <span data-ttu-id="40dbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40dbe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40dbe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40dbe-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="40dbe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40dbe-118">Request headers</span></span>
|<span data-ttu-id="40dbe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40dbe-119">Name</span></span>|<span data-ttu-id="40dbe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40dbe-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40dbe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40dbe-121">Authorization</span></span>|<span data-ttu-id="40dbe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40dbe-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="40dbe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40dbe-124">Content-Type</span></span>|<span data-ttu-id="40dbe-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40dbe-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40dbe-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="40dbe-127">Request body</span></span>
<span data-ttu-id="40dbe-128">В теле запроса укажу представление объекта [accessPackageCatalog](../resources/accesspackagecatalog.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="40dbe-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="40dbe-129">В следующей таблице показаны свойства, необходимые при обновлении [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="40dbe-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="40dbe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40dbe-130">Property</span></span>|<span data-ttu-id="40dbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40dbe-131">Type</span></span>|<span data-ttu-id="40dbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40dbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40dbe-133">displayName</span><span class="sxs-lookup"><span data-stu-id="40dbe-133">displayName</span></span>|<span data-ttu-id="40dbe-134">String</span><span class="sxs-lookup"><span data-stu-id="40dbe-134">String</span></span>|<span data-ttu-id="40dbe-135">Имя каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="40dbe-135">The access package catalog name.</span></span>|
|<span data-ttu-id="40dbe-136">description</span><span class="sxs-lookup"><span data-stu-id="40dbe-136">description</span></span>|<span data-ttu-id="40dbe-137">String</span><span class="sxs-lookup"><span data-stu-id="40dbe-137">String</span></span>|<span data-ttu-id="40dbe-138">Описание каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="40dbe-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="40dbe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="40dbe-139">Response</span></span>
<span data-ttu-id="40dbe-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40dbe-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="40dbe-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="40dbe-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40dbe-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="40dbe-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40dbe-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="40dbe-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json
Content-length: 39

{
  "displayName":"Catalog One"
}
```
# <a name="c"></a>[<span data-ttu-id="40dbe-144">C#</span><span class="sxs-lookup"><span data-stu-id="40dbe-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40dbe-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40dbe-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40dbe-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40dbe-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40dbe-147">Java</span><span class="sxs-lookup"><span data-stu-id="40dbe-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="40dbe-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="40dbe-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


