---
title: Назначение руководителя
description: Назначение руководителя пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bebf1943fb5c34f6718887f3449afb3ea5c94db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508970"
---
# <a name="assign-manager"></a><span data-ttu-id="c262a-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="c262a-103">Assign manager</span></span>

<span data-ttu-id="c262a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c262a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c262a-105">Назначение руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c262a-105">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="c262a-106">Нельзя назначать прямые отчеты; Вместо этого используйте этот API.</span><span class="sxs-lookup"><span data-stu-id="c262a-106">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c262a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c262a-107">Permissions</span></span>
<span data-ttu-id="c262a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c262a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c262a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c262a-110">Permission type</span></span>      | <span data-ttu-id="c262a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c262a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c262a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c262a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c262a-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c262a-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c262a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c262a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c262a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c262a-115">Not supported.</span></span>    |
|<span data-ttu-id="c262a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c262a-116">Application</span></span> | <span data-ttu-id="c262a-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c262a-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c262a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c262a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c262a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c262a-119">Request headers</span></span>
| <span data-ttu-id="c262a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c262a-120">Header</span></span>       | <span data-ttu-id="c262a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c262a-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c262a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c262a-122">Authorization</span></span>  | <span data-ttu-id="c262a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c262a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c262a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c262a-125">Content-type</span></span>   | <span data-ttu-id="c262a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c262a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c262a-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="c262a-128">Request body</span></span>
<span data-ttu-id="c262a-129">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [контакта Организации](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c262a-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c262a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c262a-130">Response</span></span>

<span data-ttu-id="c262a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c262a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c262a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c262a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c262a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c262a-134">Request</span></span>
<span data-ttu-id="c262a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c262a-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c262a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c262a-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c262a-137">C#</span><span class="sxs-lookup"><span data-stu-id="c262a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c262a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c262a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c262a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c262a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c262a-140">Java</span><span class="sxs-lookup"><span data-stu-id="c262a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c262a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c262a-141">Response</span></span>
<span data-ttu-id="c262a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c262a-142">The following is an example of the response.</span></span>
><span data-ttu-id="c262a-143">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c262a-143">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
