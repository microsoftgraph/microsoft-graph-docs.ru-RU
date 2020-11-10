---
title: Обновление Акцесспаккаже
description: Обновление свойств объекта Акцесспаккаже.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4fb6aa3729a4af75f5b7e416b8d577dfe43e8288
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952262"
---
# <a name="update-accesspackage"></a><span data-ttu-id="932de-103">Обновление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="932de-103">Update accessPackage</span></span>

<span data-ttu-id="932de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="932de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="932de-105">Обновление существующего объекта [акцесспаккаже](../resources/accesspackage.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="932de-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="932de-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="932de-106">Permissions</span></span>
<span data-ttu-id="932de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="932de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="932de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="932de-109">Permission type</span></span>|<span data-ttu-id="932de-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="932de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="932de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="932de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="932de-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="932de-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="932de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="932de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="932de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="932de-114">Not supported.</span></span> |
|<span data-ttu-id="932de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="932de-115">Application</span></span>                            | <span data-ttu-id="932de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="932de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="932de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="932de-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="932de-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="932de-118">Request headers</span></span>
|<span data-ttu-id="932de-119">Имя</span><span class="sxs-lookup"><span data-stu-id="932de-119">Name</span></span>|<span data-ttu-id="932de-120">Описание</span><span class="sxs-lookup"><span data-stu-id="932de-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="932de-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="932de-121">Authorization</span></span>|<span data-ttu-id="932de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="932de-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="932de-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="932de-124">Content-Type</span></span>|<span data-ttu-id="932de-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="932de-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="932de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="932de-127">Request body</span></span>
<span data-ttu-id="932de-128">В тексте запроса добавьте представление параметров объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="932de-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="932de-129">В следующей таблице приведены свойства, которые можно указать при обновлении [акцесспаккаже](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="932de-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="932de-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="932de-130">Property</span></span>|<span data-ttu-id="932de-131">Тип</span><span class="sxs-lookup"><span data-stu-id="932de-131">Type</span></span>|<span data-ttu-id="932de-132">Описание</span><span class="sxs-lookup"><span data-stu-id="932de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="932de-133">displayName</span><span class="sxs-lookup"><span data-stu-id="932de-133">displayName</span></span>|<span data-ttu-id="932de-134">String</span><span class="sxs-lookup"><span data-stu-id="932de-134">String</span></span>|<span data-ttu-id="932de-135">Имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="932de-135">The access package name.</span></span>|
|<span data-ttu-id="932de-136">description</span><span class="sxs-lookup"><span data-stu-id="932de-136">description</span></span>|<span data-ttu-id="932de-137">String</span><span class="sxs-lookup"><span data-stu-id="932de-137">String</span></span>|<span data-ttu-id="932de-138">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="932de-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="932de-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="932de-139">Response</span></span>
<span data-ttu-id="932de-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="932de-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="932de-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="932de-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="932de-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="932de-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="932de-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="932de-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="932de-144">C#</span><span class="sxs-lookup"><span data-stu-id="932de-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="932de-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="932de-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="932de-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="932de-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="932de-147">Java</span><span class="sxs-lookup"><span data-stu-id="932de-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="932de-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="932de-148">Response</span></span>

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


