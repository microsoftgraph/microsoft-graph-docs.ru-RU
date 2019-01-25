---
title: Удаление элемента без возможности восстановления
description: Окончательное удаление элемента из контейнера для удаленных элементов.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 048008e31bc5cd7884dd3d7e9259412070404d9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528202"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="9aee2-103">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="9aee2-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aee2-104">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="9aee2-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="9aee2-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="9aee2-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="9aee2-106">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="9aee2-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="9aee2-107">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="9aee2-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="9aee2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9aee2-108">Permissions</span></span>
<span data-ttu-id="9aee2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aee2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="9aee2-111">Для пользователей: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9aee2-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="9aee2-112">Для групп: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9aee2-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9aee2-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9aee2-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9aee2-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9aee2-114">Request headers</span></span>
| <span data-ttu-id="9aee2-115">Имя</span><span class="sxs-lookup"><span data-stu-id="9aee2-115">Name</span></span>       | <span data-ttu-id="9aee2-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9aee2-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9aee2-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aee2-117">Authorization</span></span>  | <span data-ttu-id="9aee2-118">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="9aee2-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="9aee2-119">Accept</span><span class="sxs-lookup"><span data-stu-id="9aee2-119">Accept</span></span>  | <span data-ttu-id="9aee2-120">application/json</span><span class="sxs-lookup"><span data-stu-id="9aee2-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9aee2-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9aee2-121">Request body</span></span>
<span data-ttu-id="9aee2-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9aee2-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9aee2-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="9aee2-123">Response</span></span>

<span data-ttu-id="9aee2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9aee2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aee2-126">Пример</span><span class="sxs-lookup"><span data-stu-id="9aee2-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9aee2-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="9aee2-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="9aee2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9aee2-128">Response</span></span>
<span data-ttu-id="9aee2-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9aee2-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
