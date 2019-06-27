---
title: Удаление участника
description: С помощью этого API можно удалить участника из группы через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 87ab921912afeeb3b094c8e30d5678741eaddd66
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275826"
---
# <a name="remove-member"></a><span data-ttu-id="28eb4-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="28eb4-103">Remove member</span></span>
<span data-ttu-id="28eb4-104">С помощью этого API можно удалить участника из группы через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="28eb4-104">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="28eb4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28eb4-105">Permissions</span></span>
<span data-ttu-id="28eb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28eb4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28eb4-108">Permission type</span></span>      | <span data-ttu-id="28eb4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28eb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28eb4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28eb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28eb4-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28eb4-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="28eb4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28eb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28eb4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28eb4-113">Not supported.</span></span> |
|<span data-ttu-id="28eb4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28eb4-114">Application</span></span> | <span data-ttu-id="28eb4-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28eb4-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28eb4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28eb4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="28eb4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28eb4-117">Request headers</span></span>
| <span data-ttu-id="28eb4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="28eb4-118">Name</span></span>       | <span data-ttu-id="28eb4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="28eb4-119">Type</span></span> | <span data-ttu-id="28eb4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="28eb4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28eb4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28eb4-121">Authorization</span></span>  | <span data-ttu-id="28eb4-122">string</span><span class="sxs-lookup"><span data-stu-id="28eb4-122">string</span></span>  | <span data-ttu-id="28eb4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28eb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28eb4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28eb4-125">Request body</span></span>
<span data-ttu-id="28eb4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28eb4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28eb4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="28eb4-127">Response</span></span>
<span data-ttu-id="28eb4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="28eb4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28eb4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="28eb4-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28eb4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="28eb4-131">Request</span></span>
<span data-ttu-id="28eb4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28eb4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="28eb4-133">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="28eb4-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="28eb4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="28eb4-134">Response</span></span>
<span data-ttu-id="28eb4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28eb4-135">The following is an example of the response.</span></span>
><span data-ttu-id="28eb4-136">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28eb4-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28eb4-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28eb4-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="28eb4-138">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="28eb4-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="28eb4-139">C#</span><span class="sxs-lookup"><span data-stu-id="28eb4-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28eb4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28eb4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="28eb4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28eb4-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
