---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7b65c4f2667e7acdb6a6ca5240df7ab68e66f594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455996"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="ccddd-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="ccddd-103">Permanently delete item</span></span>

<span data-ttu-id="ccddd-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ccddd-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ccddd-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ccddd-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="ccddd-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="ccddd-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="ccddd-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="ccddd-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccddd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccddd-108">Permissions</span></span>
<span data-ttu-id="ccddd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccddd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="ccddd-111">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="ccddd-111">For users:</span></span>

|<span data-ttu-id="ccddd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccddd-112">Permission type</span></span>      | <span data-ttu-id="ccddd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccddd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccddd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccddd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ccddd-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccddd-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ccddd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccddd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccddd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccddd-117">Not supported.</span></span> |
|<span data-ttu-id="ccddd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccddd-118">Application</span></span> | <span data-ttu-id="ccddd-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccddd-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ccddd-120">Для групп:</span><span class="sxs-lookup"><span data-stu-id="ccddd-120">For groups:</span></span>

|<span data-ttu-id="ccddd-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccddd-121">Permission type</span></span>      | <span data-ttu-id="ccddd-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccddd-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccddd-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccddd-123">Delegated (work or school account)</span></span> | <span data-ttu-id="ccddd-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccddd-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ccddd-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccddd-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccddd-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccddd-126">Not supported.</span></span>    |
|<span data-ttu-id="ccddd-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccddd-127">Application</span></span> | <span data-ttu-id="ccddd-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccddd-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccddd-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccddd-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ccddd-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccddd-130">Request headers</span></span>
| <span data-ttu-id="ccddd-131">Имя</span><span class="sxs-lookup"><span data-stu-id="ccddd-131">Name</span></span>       | <span data-ttu-id="ccddd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccddd-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ccddd-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccddd-133">Authorization</span></span>  | <span data-ttu-id="ccddd-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="ccddd-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ccddd-135">Accept</span><span class="sxs-lookup"><span data-stu-id="ccddd-135">Accept</span></span>  | <span data-ttu-id="ccddd-136">application/json</span><span class="sxs-lookup"><span data-stu-id="ccddd-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccddd-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccddd-137">Request body</span></span>
<span data-ttu-id="ccddd-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccddd-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccddd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccddd-139">Response</span></span>

<span data-ttu-id="ccddd-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ccddd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccddd-142">Пример</span><span class="sxs-lookup"><span data-stu-id="ccddd-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccddd-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccddd-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ccddd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccddd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccddd-145">C#</span><span class="sxs-lookup"><span data-stu-id="ccddd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccddd-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="ccddd-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccddd-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ccddd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccddd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccddd-148">Response</span></span>
<span data-ttu-id="ccddd-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccddd-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
