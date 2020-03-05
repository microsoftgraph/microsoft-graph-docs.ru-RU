---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 12fcd9589a35e616e20431acf0c17c6a016c4685
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420264"
---
# <a name="remove-owner"></a><span data-ttu-id="64624-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="64624-103">Remove owner</span></span>

<span data-ttu-id="64624-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64624-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64624-105">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="64624-105">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="64624-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64624-106">Permissions</span></span>
<span data-ttu-id="64624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64624-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64624-109">Permission type</span></span>      | <span data-ttu-id="64624-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64624-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64624-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64624-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64624-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64624-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64624-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64624-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64624-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64624-114">Not supported.</span></span>    |
|<span data-ttu-id="64624-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64624-115">Application</span></span> | <span data-ttu-id="64624-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64624-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64624-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64624-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="64624-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64624-118">Request headers</span></span>
| <span data-ttu-id="64624-119">Имя</span><span class="sxs-lookup"><span data-stu-id="64624-119">Name</span></span>       | <span data-ttu-id="64624-120">Тип</span><span class="sxs-lookup"><span data-stu-id="64624-120">Type</span></span> | <span data-ttu-id="64624-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64624-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64624-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64624-122">Authorization</span></span>  | <span data-ttu-id="64624-123">string</span><span class="sxs-lookup"><span data-stu-id="64624-123">string</span></span>  | <span data-ttu-id="64624-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64624-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64624-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64624-126">Request body</span></span>
<span data-ttu-id="64624-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64624-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64624-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="64624-128">Response</span></span>
<span data-ttu-id="64624-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="64624-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64624-131">Пример</span><span class="sxs-lookup"><span data-stu-id="64624-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="64624-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="64624-132">Request</span></span>
<span data-ttu-id="64624-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64624-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64624-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="64624-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="64624-135">C#</span><span class="sxs-lookup"><span data-stu-id="64624-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64624-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64624-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64624-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64624-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="64624-138">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="64624-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="64624-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="64624-139">Response</span></span>
<span data-ttu-id="64624-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64624-140">The following is an example of the response.</span></span>
><span data-ttu-id="64624-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64624-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="64624-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64624-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
