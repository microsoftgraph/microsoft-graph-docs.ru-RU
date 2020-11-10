---
title: Удаление Коннектедорганизатион
description: Удаление Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58b3ee5e9ff86c1c769689f95cf315b06c18d50c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957757"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="4a426-103">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="4a426-103">Delete connectedOrganization</span></span>

<span data-ttu-id="4a426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a426-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a426-105">Удаление объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="4a426-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a426-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a426-106">Permissions</span></span>

<span data-ttu-id="4a426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a426-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a426-109">Permission type</span></span>|<span data-ttu-id="4a426-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a426-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="4a426-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a426-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a426-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a426-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4a426-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a426-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a426-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a426-114">Not supported.</span></span> |
| <span data-ttu-id="4a426-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a426-115">Application</span></span>                            | <span data-ttu-id="4a426-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a426-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a426-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a426-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a426-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a426-118">Request headers</span></span>
|<span data-ttu-id="4a426-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a426-119">Name</span></span>|<span data-ttu-id="4a426-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a426-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4a426-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a426-121">Authorization</span></span>|<span data-ttu-id="4a426-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a426-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a426-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a426-124">Request body</span></span>
<span data-ttu-id="4a426-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a426-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a426-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a426-126">Response</span></span>

<span data-ttu-id="4a426-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a426-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4a426-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a426-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a426-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a426-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a426-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a426-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="4a426-131">C#</span><span class="sxs-lookup"><span data-stu-id="4a426-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a426-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a426-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a426-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a426-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a426-134">Java</span><span class="sxs-lookup"><span data-stu-id="4a426-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4a426-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a426-135">Response</span></span>
<span data-ttu-id="4a426-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a426-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


