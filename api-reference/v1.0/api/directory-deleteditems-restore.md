---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69594e7118e8159575b8dace0fe570a98e0d4379
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181787"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="8737e-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="8737e-103">Restore deleted item</span></span>

<span data-ttu-id="8737e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8737e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8737e-105">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8737e-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="8737e-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="8737e-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="8737e-107">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="8737e-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="8737e-108">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="8737e-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="8737e-109">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="8737e-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8737e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8737e-110">Permissions</span></span>
<span data-ttu-id="8737e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8737e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="8737e-113">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="8737e-113">For applications:</span></span>

|<span data-ttu-id="8737e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8737e-114">Permission type</span></span>      | <span data-ttu-id="8737e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8737e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8737e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8737e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8737e-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8737e-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8737e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8737e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8737e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8737e-119">Not supported.</span></span>    |
|<span data-ttu-id="8737e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8737e-120">Application</span></span> | <span data-ttu-id="8737e-121">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8737e-121">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="8737e-122">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="8737e-122">For users:</span></span>

|<span data-ttu-id="8737e-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8737e-123">Permission type</span></span>      | <span data-ttu-id="8737e-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8737e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8737e-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8737e-125">Delegated (work or school account)</span></span> | <span data-ttu-id="8737e-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8737e-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8737e-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8737e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8737e-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8737e-128">Not supported.</span></span> |
|<span data-ttu-id="8737e-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8737e-129">Application</span></span> | <span data-ttu-id="8737e-130">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8737e-130">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8737e-131">Для групп:</span><span class="sxs-lookup"><span data-stu-id="8737e-131">For groups:</span></span>

|<span data-ttu-id="8737e-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8737e-132">Permission type</span></span>      | <span data-ttu-id="8737e-133">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8737e-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8737e-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8737e-134">Delegated (work or school account)</span></span> | <span data-ttu-id="8737e-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8737e-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8737e-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8737e-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8737e-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8737e-137">Not supported.</span></span>    |
|<span data-ttu-id="8737e-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8737e-138">Application</span></span> | <span data-ttu-id="8737e-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8737e-139">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8737e-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8737e-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="8737e-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8737e-141">Request headers</span></span>
| <span data-ttu-id="8737e-142">Имя</span><span class="sxs-lookup"><span data-stu-id="8737e-142">Name</span></span>       | <span data-ttu-id="8737e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="8737e-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8737e-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="8737e-144">Authorization</span></span>  | <span data-ttu-id="8737e-145">&lt;&gt; *Необходим* маркер носителя</span><span class="sxs-lookup"><span data-stu-id="8737e-145">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="8737e-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8737e-146">Content-type</span></span> | <span data-ttu-id="8737e-147">application/json</span><span class="sxs-lookup"><span data-stu-id="8737e-147">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8737e-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8737e-148">Request body</span></span>
<span data-ttu-id="8737e-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8737e-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8737e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8737e-150">Response</span></span>

<span data-ttu-id="8737e-151">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8737e-151">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8737e-152">Пример</span><span class="sxs-lookup"><span data-stu-id="8737e-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="8737e-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="8737e-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8737e-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="8737e-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="c"></a>[<span data-ttu-id="8737e-155">C#</span><span class="sxs-lookup"><span data-stu-id="8737e-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8737e-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8737e-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8737e-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8737e-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8737e-158">Java</span><span class="sxs-lookup"><span data-stu-id="8737e-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8737e-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="8737e-159">Response</span></span>
<span data-ttu-id="8737e-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8737e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
