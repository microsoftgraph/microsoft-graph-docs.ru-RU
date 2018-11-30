---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
ms.openlocfilehash: 0f26fbe027623feac916b6af78903cdc219f167b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026088"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="0c4b8-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="0c4b8-103">Permanently delete item</span></span>

<span data-ttu-id="0c4b8-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="0c4b8-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="0c4b8-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="0c4b8-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="0c4b8-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="0c4b8-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="0c4b8-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4b8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4b8-108">Permissions</span></span>
<span data-ttu-id="0c4b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="0c4b8-111">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="0c4b8-111">For users:</span></span>

|<span data-ttu-id="0c4b8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4b8-112">Permission type</span></span>      | <span data-ttu-id="0c4b8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4b8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4b8-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c4b8-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0c4b8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-117">Not supported.</span></span> |
|<span data-ttu-id="0c4b8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4b8-118">Application</span></span> | <span data-ttu-id="0c4b8-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4b8-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="0c4b8-120">Для групп:</span><span class="sxs-lookup"><span data-stu-id="0c4b8-120">For groups:</span></span>

|<span data-ttu-id="0c4b8-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4b8-121">Permission type</span></span>      | <span data-ttu-id="0c4b8-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4b8-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4b8-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c4b8-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0c4b8-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4b8-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4b8-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-126">Not supported.</span></span>    |
|<span data-ttu-id="0c4b8-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4b8-127">Application</span></span> | <span data-ttu-id="0c4b8-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4b8-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4b8-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4b8-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0c4b8-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4b8-130">Request headers</span></span>
| <span data-ttu-id="0c4b8-131">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4b8-131">Name</span></span>       | <span data-ttu-id="0c4b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4b8-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c4b8-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c4b8-133">Authorization</span></span>  | <span data-ttu-id="0c4b8-134">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="0c4b8-135">Accept</span><span class="sxs-lookup"><span data-stu-id="0c4b8-135">Accept</span></span>  | <span data-ttu-id="0c4b8-136">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4b8-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c4b8-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c4b8-137">Request body</span></span>
<span data-ttu-id="0c4b8-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4b8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4b8-139">Response</span></span>

<span data-ttu-id="0c4b8-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4b8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4b8-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c4b8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4b8-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="0c4b8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4b8-144">Response</span></span>
<span data-ttu-id="0c4b8-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c4b8-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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