---
title: Удаление элемента
description: С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 12e26fb08f12f0cf177836baf0b5906237953f56
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263331"
---
# <a name="remove-member"></a><span data-ttu-id="fae46-104">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="fae46-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae46-105">С помощью этого API можно удалить члена группы с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="fae46-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="fae46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fae46-106">Permissions</span></span>
<span data-ttu-id="fae46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fae46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fae46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fae46-109">Permission type</span></span>      | <span data-ttu-id="fae46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fae46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fae46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fae46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fae46-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fae46-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fae46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fae46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fae46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fae46-114">Not supported.</span></span> |
|<span data-ttu-id="fae46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fae46-115">Application</span></span> | <span data-ttu-id="fae46-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fae46-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fae46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fae46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fae46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fae46-118">Request headers</span></span>
| <span data-ttu-id="fae46-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fae46-119">Name</span></span>       | <span data-ttu-id="fae46-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fae46-120">Type</span></span> | <span data-ttu-id="fae46-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fae46-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fae46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fae46-122">Authorization</span></span>  | <span data-ttu-id="fae46-123">string</span><span class="sxs-lookup"><span data-stu-id="fae46-123">string</span></span>  | <span data-ttu-id="fae46-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fae46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae46-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fae46-126">Request body</span></span>
<span data-ttu-id="fae46-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fae46-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae46-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fae46-128">Response</span></span>
<span data-ttu-id="fae46-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fae46-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fae46-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fae46-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fae46-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fae46-132">Request</span></span>
<span data-ttu-id="fae46-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fae46-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="fae46-134">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="fae46-134">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="fae46-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fae46-135">Response</span></span>
<span data-ttu-id="fae46-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fae46-136">The following is an example of the response.</span></span>
><span data-ttu-id="fae46-137">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fae46-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fae46-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fae46-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fae46-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fae46-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fae46-140">C#</span><span class="sxs-lookup"><span data-stu-id="fae46-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fae46-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="fae46-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fae46-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fae46-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
