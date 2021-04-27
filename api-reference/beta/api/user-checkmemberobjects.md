---
title: 'пользователь: checkMemberObjects'
description: Проверьте членство в списке объектов группового, каталога или административных единиц для указанного объекта пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 82ba7a3ca85f940d15dc0e16542f3129d79c2bc0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053386"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="c13b5-103">пользователь: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c13b5-103">user: checkMemberObjects</span></span>

<span data-ttu-id="c13b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13b5-105">Проверьте членство в списке объектов группового, каталога или административных единиц для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="c13b5-105">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="c13b5-106">Этот метод является транзитным.</span><span class="sxs-lookup"><span data-stu-id="c13b5-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c13b5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c13b5-107">Permissions</span></span>

<span data-ttu-id="c13b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c13b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c13b5-110">Permission type</span></span>                        | <span data-ttu-id="c13b5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c13b5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c13b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c13b5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c13b5-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c13b5-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="c13b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c13b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13b5-115">Not supported.</span></span> |
| <span data-ttu-id="c13b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c13b5-116">Application</span></span>                            | <span data-ttu-id="c13b5-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13b5-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c13b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c13b5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="c13b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c13b5-119">Request headers</span></span>

| <span data-ttu-id="c13b5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c13b5-120">Name</span></span>          | <span data-ttu-id="c13b5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c13b5-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c13b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c13b5-122">Authorization</span></span> | <span data-ttu-id="c13b5-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c13b5-123">Bearer {token}</span></span> |
| <span data-ttu-id="c13b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c13b5-124">Content-Type</span></span>  | <span data-ttu-id="c13b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c13b5-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c13b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c13b5-126">Request body</span></span>

<span data-ttu-id="c13b5-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c13b5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c13b5-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c13b5-128">Parameter</span></span>    | <span data-ttu-id="c13b5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c13b5-129">Type</span></span>        | <span data-ttu-id="c13b5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c13b5-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c13b5-131">ids</span><span class="sxs-lookup"><span data-stu-id="c13b5-131">ids</span></span>|<span data-ttu-id="c13b5-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c13b5-132">String collection</span></span>|<span data-ttu-id="c13b5-133">Коллекция, в которой содержатся объектные ИД групп, роли каталога, административные единицы или roleTemplate ID ролей каталога, в которых необходимо проверить членство.</span><span class="sxs-lookup"><span data-stu-id="c13b5-133">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="c13b5-134">Может быть указано до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="c13b5-134">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="c13b5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c13b5-135">Response</span></span>

<span data-ttu-id="c13b5-136">В случае успешной работы этот метод возвращает код отклика и новый объект `200 OK` коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c13b5-136">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c13b5-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="c13b5-137">Examples</span></span>

<span data-ttu-id="c13b5-138">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c13b5-138">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c13b5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c13b5-139">Request</span></span>

<span data-ttu-id="c13b5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c13b5-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13b5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13b5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c13b5-142">C#</span><span class="sxs-lookup"><span data-stu-id="c13b5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13b5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13b5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13b5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13b5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13b5-145">Java</span><span class="sxs-lookup"><span data-stu-id="c13b5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c13b5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c13b5-146">Response</span></span>

<span data-ttu-id="c13b5-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c13b5-147">The following is an example of the response.</span></span> 

><span data-ttu-id="c13b5-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c13b5-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


