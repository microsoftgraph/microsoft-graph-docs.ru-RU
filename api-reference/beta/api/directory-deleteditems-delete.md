---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 20179882743697a5a60ac9320a9ef552ebe44e81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437154"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="c426d-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="c426d-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c426d-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c426d-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="c426d-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c426d-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="c426d-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="c426d-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="c426d-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="c426d-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="c426d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c426d-108">Permissions</span></span>
<span data-ttu-id="c426d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c426d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c426d-111">Для пользователей: User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c426d-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="c426d-112">Для групп: Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c426d-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c426d-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c426d-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c426d-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c426d-114">Request headers</span></span>
| <span data-ttu-id="c426d-115">Имя</span><span class="sxs-lookup"><span data-stu-id="c426d-115">Name</span></span>       | <span data-ttu-id="c426d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c426d-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c426d-117">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c426d-117">Authorization</span></span>  | <span data-ttu-id="c426d-118">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="c426d-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="c426d-119">Accept</span><span class="sxs-lookup"><span data-stu-id="c426d-119">Accept</span></span>  | <span data-ttu-id="c426d-120">application/json</span><span class="sxs-lookup"><span data-stu-id="c426d-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c426d-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c426d-121">Request body</span></span>
<span data-ttu-id="c426d-122">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c426d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c426d-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="c426d-123">Response</span></span>

<span data-ttu-id="c426d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c426d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c426d-126">Пример</span><span class="sxs-lookup"><span data-stu-id="c426d-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c426d-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="c426d-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c426d-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="c426d-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c426d-129">C#</span><span class="sxs-lookup"><span data-stu-id="c426d-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c426d-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="c426d-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c426d-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c426d-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c426d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c426d-132">Response</span></span>
<span data-ttu-id="c426d-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c426d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
