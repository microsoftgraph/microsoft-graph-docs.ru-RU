---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: lleonard-msft
ms.openlocfilehash: cdea85ee1b46b4d3c7156a599081a93f31318eac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336472"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="75cfb-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="75cfb-103">Permanently delete item</span></span>

> <span data-ttu-id="75cfb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="75cfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75cfb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75cfb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75cfb-106">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="75cfb-106">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="75cfb-107">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="75cfb-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="75cfb-108">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="75cfb-108">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="75cfb-109">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="75cfb-109">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="75cfb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75cfb-110">Permissions</span></span>
<span data-ttu-id="75cfb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75cfb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="75cfb-113">Для пользователей: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75cfb-113">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="75cfb-114">Для групп: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75cfb-114">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="75cfb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75cfb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="75cfb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75cfb-116">Request headers</span></span>
| <span data-ttu-id="75cfb-117">Имя</span><span class="sxs-lookup"><span data-stu-id="75cfb-117">Name</span></span>       | <span data-ttu-id="75cfb-118">Описание</span><span class="sxs-lookup"><span data-stu-id="75cfb-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75cfb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="75cfb-119">Authorization</span></span>  | <span data-ttu-id="75cfb-120">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="75cfb-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="75cfb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="75cfb-121">Accept</span></span>  | <span data-ttu-id="75cfb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="75cfb-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="75cfb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75cfb-123">Request body</span></span>
<span data-ttu-id="75cfb-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75cfb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75cfb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="75cfb-125">Response</span></span>

<span data-ttu-id="75cfb-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75cfb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75cfb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="75cfb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75cfb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="75cfb-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="75cfb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="75cfb-130">Response</span></span>
<span data-ttu-id="75cfb-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75cfb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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