---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 68de5d829ab9b56b900af675c9ca9450688d13cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239620"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="00303-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="00303-103">Restore deleted item</span></span>

<span data-ttu-id="00303-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00303-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00303-105">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="00303-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="00303-106">В настоящее время функции восстановления удаленных элементов поддерживаются только для [приложений,](../resources/application.md) [групп и](../resources/group.md) [ресурсов](../resources/user.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="00303-106">Currently, restore deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="00303-107">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="00303-107">If an item was accidentally deleted, you can fully restore the item.</span></span> <span data-ttu-id="00303-108">Это не относится к группам безопасности, которые удаляются окончательно.</span><span class="sxs-lookup"><span data-stu-id="00303-108">This is not applicable to Security groups, which are deleted permanently.</span></span>

<span data-ttu-id="00303-109">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="00303-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="00303-110">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="00303-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="00303-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00303-111">Permissions</span></span>
<span data-ttu-id="00303-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00303-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="00303-114">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="00303-114">For applications:</span></span>

|<span data-ttu-id="00303-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00303-115">Permission type</span></span>      | <span data-ttu-id="00303-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00303-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00303-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00303-117">Delegated (work or school account)</span></span> | <span data-ttu-id="00303-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00303-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00303-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00303-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00303-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00303-120">Not supported.</span></span>    |
|<span data-ttu-id="00303-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00303-121">Application</span></span> | <span data-ttu-id="00303-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00303-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="00303-123">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="00303-123">For users:</span></span>

|<span data-ttu-id="00303-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00303-124">Permission type</span></span>      | <span data-ttu-id="00303-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00303-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00303-126">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00303-126">Delegated (work or school account)</span></span> | <span data-ttu-id="00303-127">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00303-127">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="00303-128">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00303-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00303-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00303-129">Not supported.</span></span> |
|<span data-ttu-id="00303-130">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00303-130">Application</span></span> | <span data-ttu-id="00303-131">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00303-131">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="00303-132">Для групп:</span><span class="sxs-lookup"><span data-stu-id="00303-132">For groups:</span></span>

|<span data-ttu-id="00303-133">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00303-133">Permission type</span></span>      | <span data-ttu-id="00303-134">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00303-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00303-135">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00303-135">Delegated (work or school account)</span></span> | <span data-ttu-id="00303-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00303-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="00303-137">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00303-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00303-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00303-138">Not supported.</span></span>    |
|<span data-ttu-id="00303-139">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00303-139">Application</span></span> | <span data-ttu-id="00303-140">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00303-140">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00303-141">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00303-141">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="00303-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00303-142">Request headers</span></span>
| <span data-ttu-id="00303-143">Имя</span><span class="sxs-lookup"><span data-stu-id="00303-143">Name</span></span>       | <span data-ttu-id="00303-144">Описание</span><span class="sxs-lookup"><span data-stu-id="00303-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00303-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="00303-145">Authorization</span></span>  | <span data-ttu-id="00303-146">Требуется маркер &lt; &gt; *носитела*</span><span class="sxs-lookup"><span data-stu-id="00303-146">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="00303-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00303-147">Content-type</span></span> | <span data-ttu-id="00303-148">application/json</span><span class="sxs-lookup"><span data-stu-id="00303-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="00303-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00303-149">Request body</span></span>
<span data-ttu-id="00303-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00303-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00303-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="00303-151">Response</span></span>

<span data-ttu-id="00303-152">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00303-152">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00303-153">Пример</span><span class="sxs-lookup"><span data-stu-id="00303-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="00303-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="00303-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="00303-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="00303-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="c"></a>[<span data-ttu-id="00303-156">C#</span><span class="sxs-lookup"><span data-stu-id="00303-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00303-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00303-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00303-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00303-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00303-159">Java</span><span class="sxs-lookup"><span data-stu-id="00303-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="00303-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="00303-160">Response</span></span>
<span data-ttu-id="00303-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00303-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

