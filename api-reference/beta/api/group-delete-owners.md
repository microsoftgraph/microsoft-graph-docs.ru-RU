---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9f95f242dde1447383f07508e686f42ab64b0da1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954021"
---
# <a name="remove-owner"></a><span data-ttu-id="1f1da-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="1f1da-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f1da-104">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="1f1da-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f1da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f1da-105">Permissions</span></span>
<span data-ttu-id="1f1da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f1da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f1da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f1da-108">Permission type</span></span>      | <span data-ttu-id="1f1da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f1da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f1da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f1da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f1da-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f1da-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f1da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f1da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f1da-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f1da-113">Not supported.</span></span>    |
|<span data-ttu-id="1f1da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f1da-114">Application</span></span> | <span data-ttu-id="1f1da-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f1da-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f1da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f1da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1f1da-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f1da-117">Request headers</span></span>
| <span data-ttu-id="1f1da-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1f1da-118">Name</span></span>       | <span data-ttu-id="1f1da-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1f1da-119">Type</span></span> | <span data-ttu-id="1f1da-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f1da-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f1da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f1da-121">Authorization</span></span>  | <span data-ttu-id="1f1da-122">string</span><span class="sxs-lookup"><span data-stu-id="1f1da-122">string</span></span>  | <span data-ttu-id="1f1da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f1da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f1da-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f1da-125">Request body</span></span>
<span data-ttu-id="1f1da-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f1da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f1da-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f1da-127">Response</span></span>
<span data-ttu-id="1f1da-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1f1da-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f1da-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1f1da-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f1da-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f1da-131">Request</span></span>
<span data-ttu-id="1f1da-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f1da-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f1da-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f1da-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f1da-134">C#</span><span class="sxs-lookup"><span data-stu-id="1f1da-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f1da-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f1da-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f1da-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1f1da-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f1da-137">Java</span><span class="sxs-lookup"><span data-stu-id="1f1da-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1f1da-138">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="1f1da-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="1f1da-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f1da-139">Response</span></span>
<span data-ttu-id="1f1da-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f1da-140">The following is an example of the response.</span></span>
><span data-ttu-id="1f1da-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f1da-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f1da-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f1da-142">All the properties will be returned from an actual call.</span></span>
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
