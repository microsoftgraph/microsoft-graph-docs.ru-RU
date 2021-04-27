---
title: Удаление connectorGroup
description: Удаление соединитеной группы.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d08c319f16e3f2329a0f944c1b2d313395052990
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047191"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="4a91a-103">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4a91a-103">Delete connectorGroup</span></span>

<span data-ttu-id="4a91a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a91a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a91a-105">Удаление [соединителиГруп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="4a91a-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="4a91a-106">Все [соединители](../resources/connector.md) и приложения должны быть удалены из группы соединитеителей, прежде чем группа соединитеителей может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="4a91a-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a91a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a91a-107">Permissions</span></span>
<span data-ttu-id="4a91a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a91a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a91a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a91a-110">Permission type</span></span>      | <span data-ttu-id="4a91a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a91a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a91a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a91a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a91a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a91a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a91a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a91a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a91a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a91a-115">Not supported.</span></span>    |
|<span data-ttu-id="4a91a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a91a-116">Application</span></span> | <span data-ttu-id="4a91a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a91a-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4a91a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a91a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a91a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a91a-119">Request headers</span></span>
| <span data-ttu-id="4a91a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4a91a-120">Name</span></span>       | <span data-ttu-id="4a91a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a91a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a91a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a91a-122">Authorization</span></span>  | <span data-ttu-id="4a91a-123">Носителер.</span><span class="sxs-lookup"><span data-stu-id="4a91a-123">Bearer.</span></span> <span data-ttu-id="4a91a-124">Обязательна</span><span class="sxs-lookup"><span data-stu-id="4a91a-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a91a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a91a-125">Request body</span></span>
<span data-ttu-id="4a91a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a91a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a91a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a91a-127">Response</span></span>

<span data-ttu-id="4a91a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a91a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a91a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4a91a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a91a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a91a-131">Request</span></span>
<span data-ttu-id="4a91a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a91a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a91a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a91a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="4a91a-134">C#</span><span class="sxs-lookup"><span data-stu-id="4a91a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a91a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a91a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a91a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a91a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a91a-137">Java</span><span class="sxs-lookup"><span data-stu-id="4a91a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a91a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a91a-138">Response</span></span>
<span data-ttu-id="4a91a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a91a-139">The following is an example of the response.</span></span> <span data-ttu-id="4a91a-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a91a-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



