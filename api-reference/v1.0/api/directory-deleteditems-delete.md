---
title: Постоянное удаление элемента из удаленных элементов
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 090f41ed4f6bc1410dccede72fe432e38320de0a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053211"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="8e342-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="8e342-103">Permanently delete item</span></span>

<span data-ttu-id="8e342-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e342-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e342-105">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8e342-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8e342-106">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](../resources/application.md) [групповых и](../resources/group.md) [пользовательских](../resources/user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8e342-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="8e342-107">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="8e342-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="8e342-108">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="8e342-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e342-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e342-109">Permissions</span></span>
<span data-ttu-id="8e342-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e342-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8e342-112">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="8e342-112">For applications:</span></span>

|<span data-ttu-id="8e342-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e342-113">Permission type</span></span>      | <span data-ttu-id="8e342-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e342-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e342-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e342-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8e342-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e342-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e342-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e342-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e342-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e342-118">Not supported.</span></span>    |
|<span data-ttu-id="8e342-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e342-119">Application</span></span> | <span data-ttu-id="8e342-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e342-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="8e342-121">У запросителя должна быть одна из следующих ролей: *Глобальный администратор* или *администратор приложений.*</span><span class="sxs-lookup"><span data-stu-id="8e342-121">The requestor needs to have one of the following roles: *Global Administrator* or *Application Administrator*.</span></span>

<span data-ttu-id="8e342-122">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="8e342-122">For users:</span></span>

|<span data-ttu-id="8e342-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e342-123">Permission type</span></span>      | <span data-ttu-id="8e342-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e342-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e342-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e342-125">Delegated (work or school account)</span></span> | <span data-ttu-id="8e342-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e342-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e342-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e342-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e342-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e342-128">Not supported.</span></span> |
|<span data-ttu-id="8e342-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e342-129">Application</span></span> | <span data-ttu-id="8e342-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e342-130">Not supported.</span></span> |

<span data-ttu-id="8e342-131">Пользователю, заявляемму, должна быть одна из следующих ролей: *Глобальный администратор* или *администратор пользователя.*</span><span class="sxs-lookup"><span data-stu-id="8e342-131">The signed-in user needs to have one of the following roles: *Global Administrator* or *User Administrator*.</span></span>

<span data-ttu-id="8e342-132">Для групп:</span><span class="sxs-lookup"><span data-stu-id="8e342-132">For groups:</span></span>

|<span data-ttu-id="8e342-133">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e342-133">Permission type</span></span>      | <span data-ttu-id="8e342-134">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e342-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e342-135">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e342-135">Delegated (work or school account)</span></span> | <span data-ttu-id="8e342-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e342-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e342-137">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e342-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e342-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e342-138">Not supported.</span></span>    |
|<span data-ttu-id="8e342-139">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e342-139">Application</span></span> | <span data-ttu-id="8e342-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e342-140">Not supported.</span></span> |

<span data-ttu-id="8e342-141">У запросителя должна быть одна из следующих ролей: *Глобальный администратор* или *администратор групп.*</span><span class="sxs-lookup"><span data-stu-id="8e342-141">The requestor needs to have one of the following roles: *Global Administrator* or *Groups Administrator*.</span></span>

## <a name="http-request"></a><span data-ttu-id="8e342-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e342-142">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8e342-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e342-143">Request headers</span></span>
| <span data-ttu-id="8e342-144">Имя</span><span class="sxs-lookup"><span data-stu-id="8e342-144">Name</span></span>       | <span data-ttu-id="8e342-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8e342-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e342-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e342-146">Authorization</span></span>  | <span data-ttu-id="8e342-147">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="8e342-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8e342-148">Accept</span><span class="sxs-lookup"><span data-stu-id="8e342-148">Accept</span></span>  | <span data-ttu-id="8e342-149">application/json</span><span class="sxs-lookup"><span data-stu-id="8e342-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e342-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e342-150">Request body</span></span>
<span data-ttu-id="8e342-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e342-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e342-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e342-152">Response</span></span>

<span data-ttu-id="8e342-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8e342-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e342-155">Пример</span><span class="sxs-lookup"><span data-stu-id="8e342-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e342-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e342-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8e342-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e342-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="8e342-158">C#</span><span class="sxs-lookup"><span data-stu-id="8e342-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e342-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e342-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e342-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e342-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e342-161">Java</span><span class="sxs-lookup"><span data-stu-id="8e342-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e342-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e342-162">Response</span></span>
<span data-ttu-id="8e342-163">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e342-163">Note: The response object shown here might be shortened for readability.</span></span>
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

