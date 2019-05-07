---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aac93c8f26ceb89dc1eceaa0b33e3d3d0039fef5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614861"
---
# <a name="remove-owner"></a><span data-ttu-id="dd180-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="dd180-103">Remove owner</span></span>
<span data-ttu-id="dd180-104">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="dd180-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd180-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd180-105">Permissions</span></span>
<span data-ttu-id="dd180-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd180-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd180-108">Permission type</span></span>      | <span data-ttu-id="dd180-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd180-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd180-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd180-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd180-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd180-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd180-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd180-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd180-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd180-113">Not supported.</span></span>    |
|<span data-ttu-id="dd180-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd180-114">Application</span></span> | <span data-ttu-id="dd180-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd180-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd180-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd180-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dd180-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd180-117">Request headers</span></span>
| <span data-ttu-id="dd180-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dd180-118">Name</span></span>       | <span data-ttu-id="dd180-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dd180-119">Type</span></span> | <span data-ttu-id="dd180-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd180-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd180-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd180-121">Authorization</span></span>  | <span data-ttu-id="dd180-122">string</span><span class="sxs-lookup"><span data-stu-id="dd180-122">string</span></span>  | <span data-ttu-id="dd180-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd180-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd180-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd180-125">Request body</span></span>
<span data-ttu-id="dd180-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd180-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd180-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd180-127">Response</span></span>
<span data-ttu-id="dd180-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dd180-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd180-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dd180-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dd180-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd180-131">Request</span></span>
<span data-ttu-id="dd180-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd180-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="dd180-133">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="dd180-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="dd180-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd180-134">Response</span></span>
<span data-ttu-id="dd180-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd180-135">The following is an example of the response.</span></span>
><span data-ttu-id="dd180-136">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd180-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd180-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd180-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dd180-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="dd180-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dd180-139">Языках</span><span class="sxs-lookup"><span data-stu-id="dd180-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_owner_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd180-140">Язык</span><span class="sxs-lookup"><span data-stu-id="dd180-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_owner_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
