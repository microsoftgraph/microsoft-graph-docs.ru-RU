---
title: Удаление участника
description: С помощью этого API можно удалить участника из группы через свойство навигации **members**.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 887f51eb3acf70e8eddd62e6efe507794ed382e8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783682"
---
# <a name="remove-member"></a><span data-ttu-id="b8363-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="b8363-103">Remove member</span></span>

<span data-ttu-id="b8363-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8363-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8363-105">С помощью этого API можно удалить участника из группы через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="b8363-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8363-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8363-106">Permissions</span></span>
<span data-ttu-id="b8363-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8363-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8363-109">Permission type</span></span>      | <span data-ttu-id="b8363-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8363-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8363-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8363-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b8363-112">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8363-112">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b8363-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8363-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8363-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8363-114">Not supported.</span></span> |
|<span data-ttu-id="b8363-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8363-115">Application</span></span> | <span data-ttu-id="b8363-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8363-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8363-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8363-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b8363-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8363-118">Request headers</span></span>
| <span data-ttu-id="b8363-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b8363-119">Name</span></span>       | <span data-ttu-id="b8363-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b8363-120">Type</span></span> | <span data-ttu-id="b8363-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b8363-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8363-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8363-122">Authorization</span></span>  | <span data-ttu-id="b8363-123">string</span><span class="sxs-lookup"><span data-stu-id="b8363-123">string</span></span>  | <span data-ttu-id="b8363-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8363-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8363-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8363-126">Request body</span></span>
<span data-ttu-id="b8363-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8363-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8363-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8363-128">Response</span></span>
<span data-ttu-id="b8363-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b8363-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8363-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b8363-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8363-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8363-132">Request</span></span>
<span data-ttu-id="b8363-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8363-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8363-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8363-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{group-id}/members/{directory-object-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="b8363-135">C#</span><span class="sxs-lookup"><span data-stu-id="b8363-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8363-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8363-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8363-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8363-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8363-138">Java</span><span class="sxs-lookup"><span data-stu-id="b8363-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b8363-139">В запросе укажите идентификатор группы и идентификатор объекта каталога, который вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="b8363-139">In the request, specify the identifier of the group and the identifier of the directory object you want to remove.</span></span>

#### <a name="response"></a><span data-ttu-id="b8363-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8363-140">Response</span></span>
<span data-ttu-id="b8363-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b8363-141">The following is an example of the response.</span></span>
><span data-ttu-id="b8363-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8363-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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

