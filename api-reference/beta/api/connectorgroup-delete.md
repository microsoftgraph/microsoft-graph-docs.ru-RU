---
title: Удаление connectorGroup
description: Удаление соединителиГруппы.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d5ad43b789dff0abdc7cf938746e3b75dc5f4ad4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130138"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="8bbe7-103">Удаление connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8bbe7-103">Delete connectorGroup</span></span>

<span data-ttu-id="8bbe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bbe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bbe7-105">Удаление [соединителиГруппы.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8bbe7-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="8bbe7-106">Все [соединители](../resources/connector.md) и приложения должны быть удалены из группы соединители, прежде чем можно будет удалить группу соединитеителей.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bbe7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bbe7-107">Permissions</span></span>
<span data-ttu-id="8bbe7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bbe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8bbe7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bbe7-110">Permission type</span></span>      | <span data-ttu-id="8bbe7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bbe7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bbe7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bbe7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8bbe7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bbe7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bbe7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bbe7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bbe7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-115">Not supported.</span></span>    |
|<span data-ttu-id="8bbe7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bbe7-116">Application</span></span> | <span data-ttu-id="8bbe7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8bbe7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bbe7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8bbe7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bbe7-119">Request headers</span></span>
| <span data-ttu-id="8bbe7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8bbe7-120">Name</span></span>       | <span data-ttu-id="8bbe7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbe7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8bbe7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bbe7-122">Authorization</span></span>  | <span data-ttu-id="8bbe7-123">Bearer.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-123">Bearer.</span></span> <span data-ttu-id="8bbe7-124">Обязательна</span><span class="sxs-lookup"><span data-stu-id="8bbe7-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bbe7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bbe7-125">Request body</span></span>
<span data-ttu-id="8bbe7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bbe7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bbe7-127">Response</span></span>

<span data-ttu-id="8bbe7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bbe7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8bbe7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bbe7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bbe7-131">Request</span></span>
<span data-ttu-id="8bbe7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bbe7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bbe7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="8bbe7-134">C#</span><span class="sxs-lookup"><span data-stu-id="8bbe7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bbe7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bbe7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bbe7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bbe7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bbe7-137">Java</span><span class="sxs-lookup"><span data-stu-id="8bbe7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bbe7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bbe7-138">Response</span></span>
<span data-ttu-id="8bbe7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-139">The following is an example of the response.</span></span> <span data-ttu-id="8bbe7-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8bbe7-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bbe7-141">All of the properties will be returned from an actual call.</span></span>
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



