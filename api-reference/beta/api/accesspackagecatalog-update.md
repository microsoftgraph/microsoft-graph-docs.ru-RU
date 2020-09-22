---
title: Обновление Акцесспаккажекаталог
description: Обновление свойств объекта Акцесспаккажекаталог.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3fe2af7fe7cbe2c162440ebc9204ac515fdac826
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983714"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="8b1cd-103">Обновление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="8b1cd-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="8b1cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b1cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b1cd-105">Обновление существующего объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b1cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b1cd-106">Permissions</span></span>
<span data-ttu-id="8b1cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b1cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="8b1cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b1cd-109">Permission type</span></span>|<span data-ttu-id="8b1cd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b1cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b1cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b1cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b1cd-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1cd-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="8b1cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b1cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b1cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-114">Not supported.</span></span> |
|<span data-ttu-id="8b1cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b1cd-115">Application</span></span>                            | <span data-ttu-id="8b1cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b1cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b1cd-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="8b1cd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b1cd-118">Request headers</span></span>
|<span data-ttu-id="8b1cd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b1cd-119">Name</span></span>|<span data-ttu-id="8b1cd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8b1cd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8b1cd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b1cd-121">Authorization</span></span>|<span data-ttu-id="8b1cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8b1cd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b1cd-124">Content-Type</span></span>|<span data-ttu-id="8b1cd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b1cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b1cd-127">Request body</span></span>
<span data-ttu-id="8b1cd-128">В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="8b1cd-129">В следующей таблице приведены свойства, необходимые при обновлении [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="8b1cd-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="8b1cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b1cd-130">Property</span></span>|<span data-ttu-id="8b1cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b1cd-131">Type</span></span>|<span data-ttu-id="8b1cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b1cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b1cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8b1cd-133">displayName</span></span>|<span data-ttu-id="8b1cd-134">String</span><span class="sxs-lookup"><span data-stu-id="8b1cd-134">String</span></span>|<span data-ttu-id="8b1cd-135">Имя каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-135">The access package catalog name.</span></span>|
|<span data-ttu-id="8b1cd-136">description</span><span class="sxs-lookup"><span data-stu-id="8b1cd-136">description</span></span>|<span data-ttu-id="8b1cd-137">String</span><span class="sxs-lookup"><span data-stu-id="8b1cd-137">String</span></span>|<span data-ttu-id="8b1cd-138">Описание каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="8b1cd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b1cd-139">Response</span></span>
<span data-ttu-id="8b1cd-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8b1cd-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="8b1cd-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b1cd-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b1cd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b1cd-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b1cd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1cd-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b1cd-144">C#</span><span class="sxs-lookup"><span data-stu-id="8b1cd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1cd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1cd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1cd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1cd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8b1cd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b1cd-147">Response</span></span>

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


