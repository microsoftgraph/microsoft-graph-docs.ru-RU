---
title: Удаление владельца
description: Удаление владельца приложения.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8ec6a288da6baa4dfa2d41de964a382b0e3207b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996978"
---
# <a name="remove-owner"></a><span data-ttu-id="5c599-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="5c599-103">Remove owner</span></span>

<span data-ttu-id="5c599-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c599-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c599-105">Удаление владельца из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="5c599-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c599-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c599-106">Permissions</span></span>
<span data-ttu-id="5c599-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c599-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c599-109">Permission type</span></span>      | <span data-ttu-id="5c599-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c599-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c599-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c599-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c599-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5c599-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c599-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c599-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c599-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c599-114">Not supported.</span></span>    |
|<span data-ttu-id="5c599-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c599-115">Application</span></span> | <span data-ttu-id="5c599-116">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5c599-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c599-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c599-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="5c599-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c599-118">Request headers</span></span>
| <span data-ttu-id="5c599-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c599-119">Name</span></span> | <span data-ttu-id="5c599-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c599-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="5c599-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c599-121">Authorization</span></span> | <span data-ttu-id="5c599-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c599-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c599-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c599-124">Request body</span></span>
<span data-ttu-id="5c599-125">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="5c599-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="5c599-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c599-126">Response</span></span>

<span data-ttu-id="5c599-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c599-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c599-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5c599-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c599-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c599-129">Request</span></span>

<span data-ttu-id="5c599-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c599-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c599-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c599-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="5c599-132">C#</span><span class="sxs-lookup"><span data-stu-id="5c599-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c599-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c599-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c599-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c599-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c599-135">Java</span><span class="sxs-lookup"><span data-stu-id="5c599-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c599-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c599-136">Response</span></span>

<span data-ttu-id="5c599-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c599-137">The following is an example of the response.</span></span>

><span data-ttu-id="5c599-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c599-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5c599-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c599-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


