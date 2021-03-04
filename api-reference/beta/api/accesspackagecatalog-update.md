---
title: Обновление accessPackageCatalog
description: Обновление свойств объекта accessPackageCatalog.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: de8173002582bc55aa3e59b7fbaa966240e0076e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439492"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="8a46b-103">Обновление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8a46b-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="8a46b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a46b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a46b-105">Обнови [существующий объект accessPackageCatalog,](../resources/accesspackagecatalog.md) чтобы изменить одно или несколько его свойств, например имя или описание отображения.</span><span class="sxs-lookup"><span data-stu-id="8a46b-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a46b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a46b-106">Permissions</span></span>
<span data-ttu-id="8a46b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a46b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="8a46b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a46b-109">Permission type</span></span>|<span data-ttu-id="8a46b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a46b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a46b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a46b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a46b-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a46b-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="8a46b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a46b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a46b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a46b-114">Not supported.</span></span> |
|<span data-ttu-id="8a46b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a46b-115">Application</span></span>                            | <span data-ttu-id="8a46b-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a46b-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a46b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a46b-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="8a46b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a46b-118">Request headers</span></span>
|<span data-ttu-id="8a46b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8a46b-119">Name</span></span>|<span data-ttu-id="8a46b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8a46b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a46b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a46b-121">Authorization</span></span>|<span data-ttu-id="8a46b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a46b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a46b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a46b-124">Content-Type</span></span>|<span data-ttu-id="8a46b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a46b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a46b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a46b-127">Request body</span></span>
<span data-ttu-id="8a46b-128">В теле запроса поставляем представление JSON объекта [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="8a46b-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="8a46b-129">В следующей таблице показаны свойства, необходимые при обновлении [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="8a46b-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="8a46b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a46b-130">Property</span></span>|<span data-ttu-id="8a46b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a46b-131">Type</span></span>|<span data-ttu-id="8a46b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a46b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a46b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8a46b-133">displayName</span></span>|<span data-ttu-id="8a46b-134">String</span><span class="sxs-lookup"><span data-stu-id="8a46b-134">String</span></span>|<span data-ttu-id="8a46b-135">Имя каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="8a46b-135">The access package catalog name.</span></span>|
|<span data-ttu-id="8a46b-136">description</span><span class="sxs-lookup"><span data-stu-id="8a46b-136">description</span></span>|<span data-ttu-id="8a46b-137">String</span><span class="sxs-lookup"><span data-stu-id="8a46b-137">String</span></span>|<span data-ttu-id="8a46b-138">Описание каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="8a46b-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="8a46b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a46b-139">Response</span></span>
<span data-ttu-id="8a46b-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a46b-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="8a46b-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a46b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a46b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a46b-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8a46b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a46b-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8a46b-144">C#</span><span class="sxs-lookup"><span data-stu-id="8a46b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a46b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a46b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a46b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a46b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a46b-147">Java</span><span class="sxs-lookup"><span data-stu-id="8a46b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8a46b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a46b-148">Response</span></span>

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


