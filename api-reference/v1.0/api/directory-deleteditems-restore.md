---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a0f38d24e3ba0f11ba12c59e19f933e8f7983fab
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656736"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="07861-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="07861-103">Restore deleted item</span></span>

<span data-ttu-id="07861-104">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="07861-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="07861-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="07861-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="07861-106">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="07861-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="07861-107">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="07861-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="07861-108">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="07861-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="07861-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07861-109">Permissions</span></span>
<span data-ttu-id="07861-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07861-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="07861-112">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="07861-112">For users:</span></span>

|<span data-ttu-id="07861-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07861-113">Permission type</span></span>      | <span data-ttu-id="07861-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07861-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07861-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07861-115">Delegated (work or school account)</span></span> | <span data-ttu-id="07861-116">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07861-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07861-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07861-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07861-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07861-118">Not supported.</span></span> |
|<span data-ttu-id="07861-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07861-119">Application</span></span> | <span data-ttu-id="07861-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07861-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="07861-121">Для групп:</span><span class="sxs-lookup"><span data-stu-id="07861-121">For groups:</span></span>

|<span data-ttu-id="07861-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07861-122">Permission type</span></span>      | <span data-ttu-id="07861-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07861-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07861-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07861-124">Delegated (work or school account)</span></span> | <span data-ttu-id="07861-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07861-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07861-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07861-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07861-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07861-127">Not supported.</span></span>    |
|<span data-ttu-id="07861-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07861-128">Application</span></span> | <span data-ttu-id="07861-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07861-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07861-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07861-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="07861-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07861-131">Request headers</span></span>
| <span data-ttu-id="07861-132">Имя</span><span class="sxs-lookup"><span data-stu-id="07861-132">Name</span></span>       | <span data-ttu-id="07861-133">Описание</span><span class="sxs-lookup"><span data-stu-id="07861-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07861-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07861-134">Authorization</span></span>  | <span data-ttu-id="07861-135">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="07861-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="07861-136">Accept</span><span class="sxs-lookup"><span data-stu-id="07861-136">Accept</span></span> | <span data-ttu-id="07861-137">application/json</span><span class="sxs-lookup"><span data-stu-id="07861-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="07861-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07861-138">Request body</span></span>
<span data-ttu-id="07861-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07861-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07861-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="07861-140">Response</span></span>

<span data-ttu-id="07861-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07861-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07861-142">Пример</span><span class="sxs-lookup"><span data-stu-id="07861-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07861-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="07861-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="07861-144">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07861-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07861-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="07861-145">Response</span></span>
<span data-ttu-id="07861-p104">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07861-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="07861-148">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="07861-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07861-149">C#</span><span class="sxs-lookup"><span data-stu-id="07861-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07861-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="07861-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
