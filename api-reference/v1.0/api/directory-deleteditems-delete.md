---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: lleonard-msft
ms.openlocfilehash: ef0755f757bdc2e3588acd07d86620a187002e77
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339454"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="49c80-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="49c80-103">Permanently delete item</span></span>

<span data-ttu-id="49c80-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="49c80-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="49c80-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="49c80-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="49c80-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="49c80-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="49c80-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="49c80-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="49c80-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49c80-108">Permissions</span></span>
<span data-ttu-id="49c80-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49c80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="49c80-111">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="49c80-111">For users:</span></span>

|<span data-ttu-id="49c80-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49c80-112">Permission type</span></span>      | <span data-ttu-id="49c80-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49c80-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c80-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49c80-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49c80-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49c80-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="49c80-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49c80-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c80-117">Not supported.</span></span> |
|<span data-ttu-id="49c80-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49c80-118">Application</span></span> | <span data-ttu-id="49c80-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49c80-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="49c80-120">Для групп:</span><span class="sxs-lookup"><span data-stu-id="49c80-120">For groups:</span></span>

|<span data-ttu-id="49c80-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49c80-121">Permission type</span></span>      | <span data-ttu-id="49c80-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49c80-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c80-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49c80-123">Delegated (work or school account)</span></span> | <span data-ttu-id="49c80-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49c80-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="49c80-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49c80-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c80-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c80-126">Not supported.</span></span>    |
|<span data-ttu-id="49c80-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49c80-127">Application</span></span> | <span data-ttu-id="49c80-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49c80-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49c80-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49c80-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="49c80-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49c80-130">Request headers</span></span>
| <span data-ttu-id="49c80-131">Имя</span><span class="sxs-lookup"><span data-stu-id="49c80-131">Name</span></span>       | <span data-ttu-id="49c80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49c80-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49c80-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="49c80-133">Authorization</span></span>  | <span data-ttu-id="49c80-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="49c80-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="49c80-135">Accept</span><span class="sxs-lookup"><span data-stu-id="49c80-135">Accept</span></span>  | <span data-ttu-id="49c80-136">application/json</span><span class="sxs-lookup"><span data-stu-id="49c80-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="49c80-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49c80-137">Request body</span></span>
<span data-ttu-id="49c80-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49c80-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c80-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c80-139">Response</span></span>

<span data-ttu-id="49c80-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="49c80-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c80-142">Пример</span><span class="sxs-lookup"><span data-stu-id="49c80-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49c80-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="49c80-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="49c80-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c80-144">Response</span></span>
<span data-ttu-id="49c80-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49c80-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->