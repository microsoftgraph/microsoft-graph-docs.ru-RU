---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3692e118bd7980d751f762ddc21fca556d928f6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373828"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="40f28-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="40f28-103">Restore deleted item</span></span>

<span data-ttu-id="40f28-104">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="40f28-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="40f28-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="40f28-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="40f28-106">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="40f28-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="40f28-107">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="40f28-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="40f28-108">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="40f28-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="40f28-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40f28-109">Permissions</span></span>
<span data-ttu-id="40f28-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40f28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="40f28-112">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="40f28-112">For users:</span></span>

|<span data-ttu-id="40f28-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40f28-113">Permission type</span></span>      | <span data-ttu-id="40f28-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40f28-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40f28-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40f28-115">Delegated (work or school account)</span></span> | <span data-ttu-id="40f28-116">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40f28-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="40f28-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40f28-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40f28-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40f28-118">Not supported.</span></span> |
|<span data-ttu-id="40f28-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40f28-119">Application</span></span> | <span data-ttu-id="40f28-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40f28-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="40f28-121">Для групп:</span><span class="sxs-lookup"><span data-stu-id="40f28-121">For groups:</span></span>

|<span data-ttu-id="40f28-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40f28-122">Permission type</span></span>      | <span data-ttu-id="40f28-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40f28-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40f28-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40f28-124">Delegated (work or school account)</span></span> | <span data-ttu-id="40f28-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40f28-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="40f28-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40f28-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40f28-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40f28-127">Not supported.</span></span>    |
|<span data-ttu-id="40f28-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40f28-128">Application</span></span> | <span data-ttu-id="40f28-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40f28-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40f28-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40f28-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="40f28-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40f28-131">Request headers</span></span>
| <span data-ttu-id="40f28-132">Имя</span><span class="sxs-lookup"><span data-stu-id="40f28-132">Name</span></span>       | <span data-ttu-id="40f28-133">Описание</span><span class="sxs-lookup"><span data-stu-id="40f28-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40f28-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40f28-134">Authorization</span></span>  | <span data-ttu-id="40f28-135">&lt;&gt; *Необходим* маркер носителя</span><span class="sxs-lookup"><span data-stu-id="40f28-135">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="40f28-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40f28-136">Content-type</span></span> | <span data-ttu-id="40f28-137">application/json</span><span class="sxs-lookup"><span data-stu-id="40f28-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="40f28-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40f28-138">Request body</span></span>
<span data-ttu-id="40f28-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40f28-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40f28-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="40f28-140">Response</span></span>

<span data-ttu-id="40f28-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40f28-141">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40f28-142">Пример</span><span class="sxs-lookup"><span data-stu-id="40f28-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="40f28-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="40f28-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="40f28-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="40f28-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40f28-145">C#</span><span class="sxs-lookup"><span data-stu-id="40f28-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40f28-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40f28-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40f28-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="40f28-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40f28-148">Java</span><span class="sxs-lookup"><span data-stu-id="40f28-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="40f28-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="40f28-149">Response</span></span>
<span data-ttu-id="40f28-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40f28-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
