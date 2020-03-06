---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3584d432c2300f09c53ff7107c149e8651b24b4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517245"
---
# <a name="remove-owner"></a><span data-ttu-id="9bb66-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="9bb66-103">Remove owner</span></span>

<span data-ttu-id="9bb66-104">Пространство имен: Microsoft. Graph используйте этот API, чтобы удалить владельца из группы Office 365, группы безопасности или группы безопасности с включенной поддержкой почты с помощью свойства навигации Owners.</span><span class="sxs-lookup"><span data-stu-id="9bb66-104">Namespace: microsoft.graph Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bb66-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bb66-105">Permissions</span></span>
<span data-ttu-id="9bb66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb66-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bb66-108">Permission type</span></span>      | <span data-ttu-id="9bb66-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bb66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bb66-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bb66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bb66-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bb66-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9bb66-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bb66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bb66-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bb66-113">Not supported.</span></span>    |
|<span data-ttu-id="9bb66-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bb66-114">Application</span></span> | <span data-ttu-id="9bb66-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb66-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bb66-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bb66-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9bb66-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bb66-117">Request headers</span></span>
| <span data-ttu-id="9bb66-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9bb66-118">Name</span></span>       | <span data-ttu-id="9bb66-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9bb66-119">Type</span></span> | <span data-ttu-id="9bb66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9bb66-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9bb66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb66-121">Authorization</span></span>  | <span data-ttu-id="9bb66-122">string</span><span class="sxs-lookup"><span data-stu-id="9bb66-122">string</span></span>  | <span data-ttu-id="9bb66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bb66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bb66-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bb66-125">Request body</span></span>
<span data-ttu-id="9bb66-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bb66-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bb66-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bb66-127">Response</span></span>
<span data-ttu-id="9bb66-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9bb66-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb66-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9bb66-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9bb66-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bb66-131">Request</span></span>
<span data-ttu-id="9bb66-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bb66-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bb66-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bb66-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="9bb66-134">C#</span><span class="sxs-lookup"><span data-stu-id="9bb66-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bb66-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bb66-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bb66-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bb66-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bb66-137">Java</span><span class="sxs-lookup"><span data-stu-id="9bb66-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9bb66-138">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="9bb66-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="9bb66-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bb66-139">Response</span></span>
<span data-ttu-id="9bb66-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bb66-140">The following is an example of the response.</span></span>
><span data-ttu-id="9bb66-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bb66-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9bb66-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bb66-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
