---
title: Назначение руководителя
description: Назначение руководителя пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cc9b4547e3b2e62a59f8827a88ba1e58a693aa10
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108300"
---
# <a name="assign-manager"></a><span data-ttu-id="64427-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="64427-103">Assign manager</span></span>

<span data-ttu-id="64427-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64427-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64427-105">Назначение руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="64427-105">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="64427-106">Нельзя назначать прямые отчеты; Вместо этого используйте этот API.</span><span class="sxs-lookup"><span data-stu-id="64427-106">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="64427-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64427-107">Permissions</span></span>
<span data-ttu-id="64427-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64427-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64427-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64427-110">Permission type</span></span>      | <span data-ttu-id="64427-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64427-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64427-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64427-112">Delegated (work or school account)</span></span> | <span data-ttu-id="64427-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64427-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64427-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64427-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64427-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64427-115">Not supported.</span></span>    |
|<span data-ttu-id="64427-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64427-116">Application</span></span> | <span data-ttu-id="64427-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64427-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64427-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64427-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="64427-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64427-119">Request headers</span></span>
| <span data-ttu-id="64427-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64427-120">Header</span></span>       | <span data-ttu-id="64427-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64427-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="64427-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64427-122">Authorization</span></span>  | <span data-ttu-id="64427-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64427-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64427-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64427-125">Content-type</span></span>   | <span data-ttu-id="64427-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64427-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64427-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="64427-128">Request body</span></span>
<span data-ttu-id="64427-129">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [контакта Организации](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64427-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="64427-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="64427-130">Response</span></span>

<span data-ttu-id="64427-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="64427-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64427-133">Пример</span><span class="sxs-lookup"><span data-stu-id="64427-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64427-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="64427-134">Request</span></span>
<span data-ttu-id="64427-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64427-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64427-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64427-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="64427-137">C#</span><span class="sxs-lookup"><span data-stu-id="64427-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64427-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64427-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64427-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64427-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64427-140">Java</span><span class="sxs-lookup"><span data-stu-id="64427-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64427-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="64427-141">Response</span></span>
<span data-ttu-id="64427-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64427-142">The following is an example of the response.</span></span>
><span data-ttu-id="64427-143">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64427-143">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
