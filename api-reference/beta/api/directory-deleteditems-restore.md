---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c00e117bd31960dfe1a0874c7cd5986f368b218b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963298"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="64def-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="64def-103">Restore deleted item</span></span>

<span data-ttu-id="64def-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64def-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64def-105">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="64def-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="64def-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="64def-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="64def-107">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="64def-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="64def-108">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="64def-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="64def-109">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="64def-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="64def-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64def-110">Permissions</span></span>
<span data-ttu-id="64def-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64def-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="64def-113">Для приложений:</span><span class="sxs-lookup"><span data-stu-id="64def-113">For applications:</span></span>

|<span data-ttu-id="64def-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64def-114">Permission type</span></span>      | <span data-ttu-id="64def-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64def-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64def-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64def-116">Delegated (work or school account)</span></span> | <span data-ttu-id="64def-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64def-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64def-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64def-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64def-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64def-119">Not supported.</span></span>    |
|<span data-ttu-id="64def-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64def-120">Application</span></span> | <span data-ttu-id="64def-121">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="64def-121">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |


### <a name="for-users"></a><span data-ttu-id="64def-122">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="64def-122">For users:</span></span>

|<span data-ttu-id="64def-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64def-123">Permission type</span></span>      | <span data-ttu-id="64def-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64def-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64def-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64def-125">Delegated (work or school account)</span></span> | <span data-ttu-id="64def-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64def-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="64def-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64def-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64def-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64def-128">Not supported.</span></span> |
|<span data-ttu-id="64def-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64def-129">Application</span></span> | <span data-ttu-id="64def-130">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64def-130">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="64def-131">Для групп:</span><span class="sxs-lookup"><span data-stu-id="64def-131">For groups:</span></span>

|<span data-ttu-id="64def-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64def-132">Permission type</span></span>      | <span data-ttu-id="64def-133">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64def-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64def-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64def-134">Delegated (work or school account)</span></span> | <span data-ttu-id="64def-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64def-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="64def-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64def-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64def-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64def-137">Not supported.</span></span>    |
|<span data-ttu-id="64def-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64def-138">Application</span></span> | <span data-ttu-id="64def-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64def-139">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64def-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64def-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="64def-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64def-141">Request headers</span></span>
| <span data-ttu-id="64def-142">Имя</span><span class="sxs-lookup"><span data-stu-id="64def-142">Name</span></span>       | <span data-ttu-id="64def-143">Описание</span><span class="sxs-lookup"><span data-stu-id="64def-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64def-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64def-144">Authorization</span></span>  | <span data-ttu-id="64def-145">&lt;Необходим маркер носителя &gt; *Required*</span><span class="sxs-lookup"><span data-stu-id="64def-145">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="64def-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64def-146">Content-type</span></span> | <span data-ttu-id="64def-147">application/json</span><span class="sxs-lookup"><span data-stu-id="64def-147">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="64def-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64def-148">Request body</span></span>
<span data-ttu-id="64def-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64def-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64def-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="64def-150">Response</span></span>

<span data-ttu-id="64def-151">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64def-151">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64def-152">Пример</span><span class="sxs-lookup"><span data-stu-id="64def-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="64def-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="64def-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="64def-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="64def-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="64def-155">C#</span><span class="sxs-lookup"><span data-stu-id="64def-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64def-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64def-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64def-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64def-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64def-158">Java</span><span class="sxs-lookup"><span data-stu-id="64def-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="64def-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="64def-159">Response</span></span>
<span data-ttu-id="64def-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64def-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


