---
title: Назначение руководителя
description: Назначение руководителя пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36b24ef7b6e9fb7a35be3c87723b650581ec982c
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621450"
---
# <a name="assign-manager"></a><span data-ttu-id="20f2a-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="20f2a-103">Assign manager</span></span>

<span data-ttu-id="20f2a-104">Назначение руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="20f2a-104">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="20f2a-105">Нельзя назначать прямые отчеты; Вместо этого используйте этот API.</span><span class="sxs-lookup"><span data-stu-id="20f2a-105">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="20f2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20f2a-106">Permissions</span></span>
<span data-ttu-id="20f2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20f2a-109">Permission type</span></span>      | <span data-ttu-id="20f2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20f2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20f2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20f2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20f2a-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20f2a-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20f2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20f2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20f2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f2a-114">Not supported.</span></span>    |
|<span data-ttu-id="20f2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20f2a-115">Application</span></span> | <span data-ttu-id="20f2a-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f2a-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20f2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20f2a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="20f2a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20f2a-118">Request headers</span></span>
| <span data-ttu-id="20f2a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20f2a-119">Header</span></span>       | <span data-ttu-id="20f2a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="20f2a-120">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="20f2a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20f2a-121">Authorization</span></span>  | <span data-ttu-id="20f2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20f2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20f2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20f2a-124">Content-type</span></span>   | <span data-ttu-id="20f2a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20f2a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20f2a-127">Request body</span></span>
<span data-ttu-id="20f2a-128">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [контакта Организации](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20f2a-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="20f2a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="20f2a-129">Response</span></span>

<span data-ttu-id="20f2a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="20f2a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f2a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="20f2a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20f2a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="20f2a-133">Request</span></span>
<span data-ttu-id="20f2a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20f2a-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20f2a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="20f2a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20f2a-136">C#</span><span class="sxs-lookup"><span data-stu-id="20f2a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20f2a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20f2a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20f2a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20f2a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="20f2a-139">Java</span><span class="sxs-lookup"><span data-stu-id="20f2a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20f2a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="20f2a-140">Response</span></span>
<span data-ttu-id="20f2a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20f2a-141">The following is an example of the response.</span></span>
><span data-ttu-id="20f2a-142">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20f2a-142">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
