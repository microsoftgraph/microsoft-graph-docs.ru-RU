---
title: Удаление Коннектедорганизатион
description: Удаление Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b26e7a2d872e75217a0a4fc0a40e9e88df197310
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996537"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="5eaf3-103">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5eaf3-103">Delete connectedOrganization</span></span>

<span data-ttu-id="5eaf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eaf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eaf3-105">Удаление объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="5eaf3-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eaf3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5eaf3-106">Permissions</span></span>

<span data-ttu-id="5eaf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eaf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eaf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eaf3-109">Permission type</span></span>|<span data-ttu-id="5eaf3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eaf3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="5eaf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eaf3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5eaf3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eaf3-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5eaf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eaf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eaf3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-114">Not supported.</span></span> |
| <span data-ttu-id="5eaf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eaf3-115">Application</span></span>                            | <span data-ttu-id="5eaf3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eaf3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eaf3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5eaf3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eaf3-118">Request headers</span></span>
|<span data-ttu-id="5eaf3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5eaf3-119">Name</span></span>|<span data-ttu-id="5eaf3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5eaf3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5eaf3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eaf3-121">Authorization</span></span>|<span data-ttu-id="5eaf3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eaf3-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5eaf3-124">Request body</span></span>
<span data-ttu-id="5eaf3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eaf3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eaf3-126">Response</span></span>

<span data-ttu-id="5eaf3-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5eaf3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5eaf3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5eaf3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eaf3-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5eaf3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eaf3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="5eaf3-131">C#</span><span class="sxs-lookup"><span data-stu-id="5eaf3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eaf3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eaf3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eaf3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eaf3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5eaf3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eaf3-134">Response</span></span>
<span data-ttu-id="5eaf3-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5eaf3-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


