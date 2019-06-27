---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d806b879fce8a7352576684a3f3254a25e777863
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276883"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="a43b2-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="a43b2-103">Permanently delete item</span></span>

<span data-ttu-id="a43b2-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a43b2-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a43b2-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a43b2-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="a43b2-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="a43b2-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="a43b2-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="a43b2-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="a43b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a43b2-108">Permissions</span></span>
<span data-ttu-id="a43b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a43b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="a43b2-111">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="a43b2-111">For users:</span></span>

|<span data-ttu-id="a43b2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a43b2-112">Permission type</span></span>      | <span data-ttu-id="a43b2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a43b2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a43b2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a43b2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a43b2-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a43b2-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a43b2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a43b2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a43b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43b2-117">Not supported.</span></span> |
|<span data-ttu-id="a43b2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a43b2-118">Application</span></span> | <span data-ttu-id="a43b2-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a43b2-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="a43b2-120">Для групп:</span><span class="sxs-lookup"><span data-stu-id="a43b2-120">For groups:</span></span>

|<span data-ttu-id="a43b2-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a43b2-121">Permission type</span></span>      | <span data-ttu-id="a43b2-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a43b2-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a43b2-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a43b2-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a43b2-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a43b2-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a43b2-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a43b2-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a43b2-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43b2-126">Not supported.</span></span>    |
|<span data-ttu-id="a43b2-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a43b2-127">Application</span></span> | <span data-ttu-id="a43b2-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a43b2-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a43b2-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a43b2-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a43b2-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a43b2-130">Request headers</span></span>
| <span data-ttu-id="a43b2-131">Имя</span><span class="sxs-lookup"><span data-stu-id="a43b2-131">Name</span></span>       | <span data-ttu-id="a43b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a43b2-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a43b2-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a43b2-133">Authorization</span></span>  | <span data-ttu-id="a43b2-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="a43b2-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a43b2-135">Accept</span><span class="sxs-lookup"><span data-stu-id="a43b2-135">Accept</span></span>  | <span data-ttu-id="a43b2-136">application/json</span><span class="sxs-lookup"><span data-stu-id="a43b2-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a43b2-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a43b2-137">Request body</span></span>
<span data-ttu-id="a43b2-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a43b2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a43b2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a43b2-139">Response</span></span>

<span data-ttu-id="a43b2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a43b2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a43b2-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a43b2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a43b2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a43b2-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="a43b2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a43b2-144">Response</span></span>
<span data-ttu-id="a43b2-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a43b2-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a43b2-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a43b2-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a43b2-148">C#</span><span class="sxs-lookup"><span data-stu-id="a43b2-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a43b2-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="a43b2-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a43b2-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a43b2-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
