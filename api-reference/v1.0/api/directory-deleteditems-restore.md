---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06f58e436d0e4b2225013cda90c45d51a7da23cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941935"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="6dcd4-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="6dcd4-103">Restore deleted item</span></span>

<span data-ttu-id="6dcd4-104">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6dcd4-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="6dcd4-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="6dcd4-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="6dcd4-106">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="6dcd4-107">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="6dcd4-108">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dcd4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcd4-109">Permissions</span></span>
<span data-ttu-id="6dcd4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dcd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="6dcd4-112">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="6dcd4-112">For users:</span></span>

|<span data-ttu-id="6dcd4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcd4-113">Permission type</span></span>      | <span data-ttu-id="6dcd4-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dcd4-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6dcd4-116">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dcd4-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6dcd4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dcd4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-118">Not supported.</span></span> |
|<span data-ttu-id="6dcd4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dcd4-119">Application</span></span> | <span data-ttu-id="6dcd4-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dcd4-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="6dcd4-121">Для групп:</span><span class="sxs-lookup"><span data-stu-id="6dcd4-121">For groups:</span></span>

|<span data-ttu-id="6dcd4-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcd4-122">Permission type</span></span>      | <span data-ttu-id="6dcd4-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dcd4-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-124">Delegated (work or school account)</span></span> | <span data-ttu-id="6dcd4-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dcd4-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6dcd4-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dcd4-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dcd4-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-127">Not supported.</span></span>    |
|<span data-ttu-id="6dcd4-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dcd4-128">Application</span></span> | <span data-ttu-id="6dcd4-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dcd4-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dcd4-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dcd4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="6dcd4-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dcd4-131">Request headers</span></span>
| <span data-ttu-id="6dcd4-132">Имя</span><span class="sxs-lookup"><span data-stu-id="6dcd4-132">Name</span></span>       | <span data-ttu-id="6dcd4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6dcd4-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6dcd4-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dcd4-134">Authorization</span></span>  | <span data-ttu-id="6dcd4-135">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="6dcd4-136">Accept</span><span class="sxs-lookup"><span data-stu-id="6dcd4-136">Accept</span></span> | <span data-ttu-id="6dcd4-137">application/json</span><span class="sxs-lookup"><span data-stu-id="6dcd4-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dcd4-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6dcd4-138">Request body</span></span>
<span data-ttu-id="6dcd4-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dcd4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcd4-140">Response</span></span>

<span data-ttu-id="6dcd4-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dcd4-142">Пример</span><span class="sxs-lookup"><span data-stu-id="6dcd4-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dcd4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dcd4-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="6dcd4-144">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6dcd4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcd4-145">Response</span></span>
<span data-ttu-id="6dcd4-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dcd4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
