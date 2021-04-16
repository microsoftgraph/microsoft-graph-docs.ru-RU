---
title: 'пользователь: checkMemberObjects'
description: Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: df3cf26e98f3769bea4ceba632dccd24030494b0
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870067"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="49942-103">пользователь: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="49942-103">user: checkMemberObjects</span></span>

<span data-ttu-id="49942-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49942-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49942-105">Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="49942-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="49942-106">Этот метод является транзитным.</span><span class="sxs-lookup"><span data-stu-id="49942-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="49942-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49942-107">Permissions</span></span>

<span data-ttu-id="49942-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49942-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49942-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49942-110">Permission type</span></span>                        | <span data-ttu-id="49942-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49942-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49942-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49942-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49942-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49942-113">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="49942-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49942-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49942-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49942-115">Not supported.</span></span> |
| <span data-ttu-id="49942-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49942-116">Application</span></span>                            | <span data-ttu-id="49942-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49942-117">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49942-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49942-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="49942-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49942-119">Request headers</span></span>

| <span data-ttu-id="49942-120">Имя</span><span class="sxs-lookup"><span data-stu-id="49942-120">Name</span></span>          | <span data-ttu-id="49942-121">Описание</span><span class="sxs-lookup"><span data-stu-id="49942-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49942-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49942-122">Authorization</span></span> | <span data-ttu-id="49942-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49942-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49942-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49942-125">Content-Type</span></span>  | <span data-ttu-id="49942-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49942-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49942-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49942-128">Request body</span></span>

<span data-ttu-id="49942-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="49942-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49942-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="49942-130">Parameter</span></span>    | <span data-ttu-id="49942-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49942-131">Type</span></span>        | <span data-ttu-id="49942-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49942-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49942-133">ids</span><span class="sxs-lookup"><span data-stu-id="49942-133">ids</span></span>|<span data-ttu-id="49942-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49942-134">String collection</span></span>|<span data-ttu-id="49942-135">Коллекция, которая содержит объектные ID групп, роли каталога или roleTemplate ID ролей каталога, в которых необходимо проверить членство.</span><span class="sxs-lookup"><span data-stu-id="49942-135">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="49942-136">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="49942-136">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="49942-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="49942-137">Response</span></span>

<span data-ttu-id="49942-138">В случае успешной работы этот метод возвращает код отклика и новый объект `200 OK` коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49942-138">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49942-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="49942-139">Examples</span></span>

<span data-ttu-id="49942-140">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49942-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="49942-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="49942-141">Request</span></span>

<span data-ttu-id="49942-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49942-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49942-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="49942-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="49942-144">C#</span><span class="sxs-lookup"><span data-stu-id="49942-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49942-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49942-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49942-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49942-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49942-147">Java</span><span class="sxs-lookup"><span data-stu-id="49942-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49942-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="49942-148">Response</span></span>

<span data-ttu-id="49942-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49942-149">The following is an example of the response.</span></span> 

><span data-ttu-id="49942-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49942-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

