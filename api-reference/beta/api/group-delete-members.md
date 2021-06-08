---
title: Удаление участника
description: Используйте этот API, чтобы удалить участника из группы Microsoft 365, группы безопасности или группы  безопасности с поддержкой почты через свойство навигации членов. Вы можете удалять пользователей или другие группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5950e65c02301bbd6379b0860d418692ed2f0721
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786967"
---
# <a name="remove-member"></a><span data-ttu-id="4c51b-104">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="4c51b-104">Remove member</span></span>

<span data-ttu-id="4c51b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c51b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c51b-106">С помощью этого API можно удалить участника из группы через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="4c51b-106">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c51b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c51b-107">Permissions</span></span>
<span data-ttu-id="4c51b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c51b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c51b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c51b-110">Permission type</span></span>      | <span data-ttu-id="4c51b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c51b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c51b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c51b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c51b-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c51b-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4c51b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c51b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c51b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c51b-115">Not supported.</span></span> |
|<span data-ttu-id="4c51b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c51b-116">Application</span></span> | <span data-ttu-id="4c51b-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c51b-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c51b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c51b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4c51b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c51b-119">Request headers</span></span>
| <span data-ttu-id="4c51b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4c51b-120">Name</span></span>       | <span data-ttu-id="4c51b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c51b-121">Type</span></span> | <span data-ttu-id="4c51b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c51b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c51b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c51b-123">Authorization</span></span>  | <span data-ttu-id="4c51b-124">string</span><span class="sxs-lookup"><span data-stu-id="4c51b-124">string</span></span>  | <span data-ttu-id="4c51b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c51b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c51b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c51b-127">Request body</span></span>
<span data-ttu-id="4c51b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c51b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c51b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c51b-129">Response</span></span>
<span data-ttu-id="4c51b-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c51b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c51b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4c51b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4c51b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c51b-133">Request</span></span>
<span data-ttu-id="4c51b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c51b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c51b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c51b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{group-id}/members/{directory-object-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="4c51b-136">C#</span><span class="sxs-lookup"><span data-stu-id="4c51b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c51b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c51b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c51b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c51b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c51b-139">Java</span><span class="sxs-lookup"><span data-stu-id="4c51b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4c51b-140">В запросе укажите идентификатор группы и идентификатор объекта каталога, который вы хотите удалить.</span><span class="sxs-lookup"><span data-stu-id="4c51b-140">In the request, specify the identifier of the group and the identifier of the directory object you want to remove.</span></span>

#### <a name="response"></a><span data-ttu-id="4c51b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c51b-141">Response</span></span>
<span data-ttu-id="4c51b-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c51b-142">The following is an example of the response.</span></span>
><span data-ttu-id="4c51b-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c51b-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->


