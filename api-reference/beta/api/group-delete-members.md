---
title: Удаление элемента
description: С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7840cd40f56e1a43b74219c29be810f684246e37
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858943"
---
# <a name="remove-member"></a><span data-ttu-id="551ce-104">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="551ce-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="551ce-105">С помощью этого API можно удалить члена группы с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="551ce-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="551ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="551ce-106">Permissions</span></span>
<span data-ttu-id="551ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="551ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="551ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="551ce-109">Permission type</span></span>      | <span data-ttu-id="551ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="551ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="551ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="551ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="551ce-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="551ce-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="551ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="551ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="551ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="551ce-114">Not supported.</span></span> |
|<span data-ttu-id="551ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="551ce-115">Application</span></span> | <span data-ttu-id="551ce-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="551ce-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="551ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="551ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="551ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="551ce-118">Request headers</span></span>
| <span data-ttu-id="551ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="551ce-119">Name</span></span>       | <span data-ttu-id="551ce-120">Тип</span><span class="sxs-lookup"><span data-stu-id="551ce-120">Type</span></span> | <span data-ttu-id="551ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="551ce-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="551ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="551ce-122">Authorization</span></span>  | <span data-ttu-id="551ce-123">string</span><span class="sxs-lookup"><span data-stu-id="551ce-123">string</span></span>  | <span data-ttu-id="551ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="551ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="551ce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="551ce-126">Request body</span></span>
<span data-ttu-id="551ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="551ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="551ce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="551ce-128">Response</span></span>
<span data-ttu-id="551ce-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="551ce-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="551ce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="551ce-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="551ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="551ce-132">Request</span></span>
<span data-ttu-id="551ce-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="551ce-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="551ce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="551ce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="551ce-135">C#</span><span class="sxs-lookup"><span data-stu-id="551ce-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="551ce-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="551ce-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="551ce-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="551ce-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="551ce-138">Java</span><span class="sxs-lookup"><span data-stu-id="551ce-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="551ce-139">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="551ce-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="551ce-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="551ce-140">Response</span></span>
<span data-ttu-id="551ce-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="551ce-141">The following is an example of the response.</span></span>
><span data-ttu-id="551ce-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="551ce-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="551ce-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="551ce-143">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
