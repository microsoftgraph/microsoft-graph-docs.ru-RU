---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f4bcdcc1f826a3f6a4f176564042b54f065de54
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374021"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="d9c13-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="d9c13-103">Permanently delete item</span></span>

<span data-ttu-id="d9c13-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="d9c13-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="d9c13-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d9c13-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="d9c13-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="d9c13-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="d9c13-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="d9c13-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9c13-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9c13-108">Permissions</span></span>
<span data-ttu-id="d9c13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9c13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="d9c13-111">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="d9c13-111">For users:</span></span>

|<span data-ttu-id="d9c13-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9c13-112">Permission type</span></span>      | <span data-ttu-id="d9c13-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9c13-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9c13-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9c13-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d9c13-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9c13-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d9c13-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9c13-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9c13-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9c13-117">Not supported.</span></span> |
|<span data-ttu-id="d9c13-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9c13-118">Application</span></span> | <span data-ttu-id="d9c13-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c13-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="d9c13-120">Для групп:</span><span class="sxs-lookup"><span data-stu-id="d9c13-120">For groups:</span></span>

|<span data-ttu-id="d9c13-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9c13-121">Permission type</span></span>      | <span data-ttu-id="d9c13-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9c13-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9c13-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9c13-123">Delegated (work or school account)</span></span> | <span data-ttu-id="d9c13-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9c13-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d9c13-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9c13-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9c13-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9c13-126">Not supported.</span></span>    |
|<span data-ttu-id="d9c13-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9c13-127">Application</span></span> | <span data-ttu-id="d9c13-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c13-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9c13-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9c13-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d9c13-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9c13-130">Request headers</span></span>
| <span data-ttu-id="d9c13-131">Имя</span><span class="sxs-lookup"><span data-stu-id="d9c13-131">Name</span></span>       | <span data-ttu-id="d9c13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9c13-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9c13-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9c13-133">Authorization</span></span>  | <span data-ttu-id="d9c13-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="d9c13-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="d9c13-135">Accept</span><span class="sxs-lookup"><span data-stu-id="d9c13-135">Accept</span></span>  | <span data-ttu-id="d9c13-136">application/json</span><span class="sxs-lookup"><span data-stu-id="d9c13-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9c13-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9c13-137">Request body</span></span>
<span data-ttu-id="d9c13-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9c13-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9c13-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9c13-139">Response</span></span>

<span data-ttu-id="d9c13-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9c13-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9c13-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d9c13-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9c13-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9c13-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d9c13-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c13-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9c13-145">C#</span><span class="sxs-lookup"><span data-stu-id="d9c13-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9c13-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9c13-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9c13-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d9c13-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d9c13-148">Java</span><span class="sxs-lookup"><span data-stu-id="d9c13-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9c13-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9c13-149">Response</span></span>
<span data-ttu-id="d9c13-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9c13-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
