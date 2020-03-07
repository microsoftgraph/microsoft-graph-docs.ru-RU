---
title: Удаление участника
description: С помощью этого API можно удалить участника из группы через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 54066ba22f34481bd213806909dc0f826d6860d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517196"
---
# <a name="remove-member"></a><span data-ttu-id="a6c79-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="a6c79-103">Remove member</span></span>

<span data-ttu-id="a6c79-104">Пространство имен: microsoft.graph С помощью этого API можно удалить участника из группы через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-104">Namespace: microsoft.graph Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c79-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c79-105">Permissions</span></span>
<span data-ttu-id="a6c79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c79-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c79-108">Permission type</span></span>      | <span data-ttu-id="a6c79-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6c79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c79-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6c79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c79-111">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6c79-111">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a6c79-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6c79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c79-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c79-113">Not supported.</span></span> |
|<span data-ttu-id="a6c79-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="a6c79-114">Application</span></span> | <span data-ttu-id="a6c79-115">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c79-115">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c79-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6c79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a6c79-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6c79-117">Request headers</span></span>
| <span data-ttu-id="a6c79-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a6c79-118">Name</span></span>       | <span data-ttu-id="a6c79-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c79-119">Type</span></span> | <span data-ttu-id="a6c79-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c79-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6c79-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c79-121">Authorization</span></span>  | <span data-ttu-id="a6c79-122">string</span><span class="sxs-lookup"><span data-stu-id="a6c79-122">string</span></span>  | <span data-ttu-id="a6c79-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6c79-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c79-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6c79-125">Request body</span></span>
<span data-ttu-id="a6c79-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6c79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c79-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c79-127">Response</span></span>
<span data-ttu-id="a6c79-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a6c79-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c79-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a6c79-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a6c79-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6c79-131">Request</span></span>
<span data-ttu-id="a6c79-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6c79-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6c79-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c79-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="a6c79-134">C#</span><span class="sxs-lookup"><span data-stu-id="a6c79-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6c79-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6c79-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6c79-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6c79-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6c79-137">Java</span><span class="sxs-lookup"><span data-stu-id="a6c79-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a6c79-138">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="a6c79-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="a6c79-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c79-139">Response</span></span>
<span data-ttu-id="a6c79-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c79-140">The following is an example of the response.</span></span>
><span data-ttu-id="a6c79-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a6c79-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6c79-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6c79-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
