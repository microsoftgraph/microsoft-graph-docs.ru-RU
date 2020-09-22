---
title: Обновление Акцесспаккаже
description: Обновление свойств объекта Акцесспаккаже.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04497ffcaeb8a7c738d18aff9e6668712cab4ace
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983930"
---
# <a name="update-accesspackage"></a><span data-ttu-id="d557e-103">Обновление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d557e-103">Update accessPackage</span></span>

<span data-ttu-id="d557e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d557e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d557e-105">Обновление существующего объекта [акцесспаккаже](../resources/accesspackage.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="d557e-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="d557e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d557e-106">Permissions</span></span>
<span data-ttu-id="d557e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d557e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d557e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d557e-109">Permission type</span></span>|<span data-ttu-id="d557e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d557e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d557e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d557e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d557e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d557e-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="d557e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d557e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d557e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d557e-114">Not supported.</span></span> |
|<span data-ttu-id="d557e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d557e-115">Application</span></span>                            | <span data-ttu-id="d557e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d557e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d557e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d557e-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="d557e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d557e-118">Request headers</span></span>
|<span data-ttu-id="d557e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d557e-119">Name</span></span>|<span data-ttu-id="d557e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d557e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d557e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d557e-121">Authorization</span></span>|<span data-ttu-id="d557e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d557e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d557e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d557e-124">Content-Type</span></span>|<span data-ttu-id="d557e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d557e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d557e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d557e-127">Request body</span></span>
<span data-ttu-id="d557e-128">В тексте запроса добавьте представление параметров объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d557e-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="d557e-129">В следующей таблице приведены свойства, которые можно указать при обновлении [акцесспаккаже](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="d557e-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="d557e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d557e-130">Property</span></span>|<span data-ttu-id="d557e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d557e-131">Type</span></span>|<span data-ttu-id="d557e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d557e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d557e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d557e-133">displayName</span></span>|<span data-ttu-id="d557e-134">String</span><span class="sxs-lookup"><span data-stu-id="d557e-134">String</span></span>|<span data-ttu-id="d557e-135">Имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d557e-135">The access package name.</span></span>|
|<span data-ttu-id="d557e-136">description</span><span class="sxs-lookup"><span data-stu-id="d557e-136">description</span></span>|<span data-ttu-id="d557e-137">String</span><span class="sxs-lookup"><span data-stu-id="d557e-137">String</span></span>|<span data-ttu-id="d557e-138">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d557e-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="d557e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d557e-139">Response</span></span>
<span data-ttu-id="d557e-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d557e-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d557e-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="d557e-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d557e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d557e-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d557e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d557e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json
Content-length: 38

{
  "displayName":"Access Package New Name"
}
```
# <a name="c"></a>[<span data-ttu-id="d557e-144">C#</span><span class="sxs-lookup"><span data-stu-id="d557e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d557e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d557e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d557e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d557e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d557e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d557e-147">Response</span></span>

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
  "description": "Update accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


