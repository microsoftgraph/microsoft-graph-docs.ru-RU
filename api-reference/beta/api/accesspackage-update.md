---
title: Обновление accessPackage
description: Обновление свойств объекта accessPackage.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 40f299edcca636a6f2041a36e10b0dc3963d8422
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439767"
---
# <a name="update-accesspackage"></a><span data-ttu-id="6a667-103">Обновление accessPackage</span><span class="sxs-lookup"><span data-stu-id="6a667-103">Update accessPackage</span></span>

<span data-ttu-id="6a667-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a667-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a667-105">Обновим [существующий объект accessPackage,](../resources/accesspackage.md) чтобы изменить одно или несколько его свойств, например имя или описание отображения.</span><span class="sxs-lookup"><span data-stu-id="6a667-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a667-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a667-106">Permissions</span></span>
<span data-ttu-id="6a667-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="6a667-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a667-109">Permission type</span></span>|<span data-ttu-id="6a667-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a667-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a667-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a667-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a667-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a667-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="6a667-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a667-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a667-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a667-114">Not supported.</span></span> |
|<span data-ttu-id="6a667-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a667-115">Application</span></span>                            | <span data-ttu-id="6a667-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a667-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a667-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a667-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="6a667-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a667-118">Request headers</span></span>
|<span data-ttu-id="6a667-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6a667-119">Name</span></span>|<span data-ttu-id="6a667-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a667-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a667-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a667-121">Authorization</span></span>|<span data-ttu-id="6a667-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a667-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6a667-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a667-124">Content-Type</span></span>|<span data-ttu-id="6a667-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a667-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a667-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a667-127">Request body</span></span>
<span data-ttu-id="6a667-128">В теле запроса поставляем представление JSON параметров [объекта accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="6a667-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="6a667-129">В следующей таблице показаны свойства, которые можно получить при обновлении [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="6a667-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="6a667-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a667-130">Property</span></span>|<span data-ttu-id="6a667-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6a667-131">Type</span></span>|<span data-ttu-id="6a667-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6a667-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a667-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6a667-133">displayName</span></span>|<span data-ttu-id="6a667-134">String</span><span class="sxs-lookup"><span data-stu-id="6a667-134">String</span></span>|<span data-ttu-id="6a667-135">Имя пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="6a667-135">The access package name.</span></span>|
|<span data-ttu-id="6a667-136">description</span><span class="sxs-lookup"><span data-stu-id="6a667-136">description</span></span>|<span data-ttu-id="6a667-137">String</span><span class="sxs-lookup"><span data-stu-id="6a667-137">String</span></span>|<span data-ttu-id="6a667-138">Описание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="6a667-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="6a667-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a667-139">Response</span></span>
<span data-ttu-id="6a667-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6a667-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6a667-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a667-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a667-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a667-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6a667-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a667-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6a667-144">C#</span><span class="sxs-lookup"><span data-stu-id="6a667-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a667-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a667-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a667-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a667-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a667-147">Java</span><span class="sxs-lookup"><span data-stu-id="6a667-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6a667-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a667-148">Response</span></span>

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


