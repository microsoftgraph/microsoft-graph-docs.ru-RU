---
title: Окончательное удаление элемента из удаленных элементов
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da494a4cb456119e0a0e2f3ac51fa57531394331
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239102"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="edd38-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="edd38-103">Permanently delete item</span></span>

<span data-ttu-id="edd38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edd38-105">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="edd38-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="edd38-106">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](../resources/application.md) [групп и](../resources/group.md) [пользовательских](../resources/user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="edd38-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="edd38-107">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="edd38-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="edd38-108">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="edd38-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="edd38-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edd38-109">Permissions</span></span>
<span data-ttu-id="edd38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edd38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="edd38-112">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="edd38-112">For applications:</span></span>

|<span data-ttu-id="edd38-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edd38-113">Permission type</span></span>      | <span data-ttu-id="edd38-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edd38-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd38-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edd38-115">Delegated (work or school account)</span></span> | <span data-ttu-id="edd38-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd38-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edd38-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edd38-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd38-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd38-118">Not supported.</span></span>    |
|<span data-ttu-id="edd38-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edd38-119">Application</span></span> | <span data-ttu-id="edd38-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edd38-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="edd38-121">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="edd38-121">For users:</span></span>

|<span data-ttu-id="edd38-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edd38-122">Permission type</span></span>      | <span data-ttu-id="edd38-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edd38-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd38-124">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edd38-124">Delegated (work or school account)</span></span> | <span data-ttu-id="edd38-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd38-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="edd38-126">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edd38-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd38-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd38-127">Not supported.</span></span> |
|<span data-ttu-id="edd38-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edd38-128">Application</span></span> | <span data-ttu-id="edd38-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd38-129">Not supported.</span></span> |

<span data-ttu-id="edd38-130">Для групп:</span><span class="sxs-lookup"><span data-stu-id="edd38-130">For groups:</span></span>

|<span data-ttu-id="edd38-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edd38-131">Permission type</span></span>      | <span data-ttu-id="edd38-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edd38-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd38-133">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edd38-133">Delegated (work or school account)</span></span> | <span data-ttu-id="edd38-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd38-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="edd38-135">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edd38-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd38-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd38-136">Not supported.</span></span>    |
|<span data-ttu-id="edd38-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edd38-137">Application</span></span> | <span data-ttu-id="edd38-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd38-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edd38-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edd38-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="edd38-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edd38-140">Request headers</span></span>
| <span data-ttu-id="edd38-141">Имя</span><span class="sxs-lookup"><span data-stu-id="edd38-141">Name</span></span>       | <span data-ttu-id="edd38-142">Описание</span><span class="sxs-lookup"><span data-stu-id="edd38-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="edd38-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="edd38-143">Authorization</span></span>  | <span data-ttu-id="edd38-144">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="edd38-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="edd38-145">Accept</span><span class="sxs-lookup"><span data-stu-id="edd38-145">Accept</span></span>  | <span data-ttu-id="edd38-146">application/json</span><span class="sxs-lookup"><span data-stu-id="edd38-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="edd38-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edd38-147">Request body</span></span>
<span data-ttu-id="edd38-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edd38-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edd38-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="edd38-149">Response</span></span>

<span data-ttu-id="edd38-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="edd38-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edd38-152">Пример</span><span class="sxs-lookup"><span data-stu-id="edd38-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edd38-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="edd38-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="edd38-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd38-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="edd38-155">C#</span><span class="sxs-lookup"><span data-stu-id="edd38-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd38-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd38-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd38-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd38-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edd38-158">Java</span><span class="sxs-lookup"><span data-stu-id="edd38-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="edd38-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="edd38-159">Response</span></span>
<span data-ttu-id="edd38-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edd38-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

