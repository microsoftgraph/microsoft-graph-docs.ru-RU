---
title: 'user: getMemberObjects'
description: Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8a140e0cde1497e864b82b54af398c285952b3ae
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055675"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="eafe3-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="eafe3-104">user: getMemberObjects</span></span>

<span data-ttu-id="eafe3-p102">Пространство имен: microsoft.graph. Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="eafe3-p102">Namespace: microsoft.graph Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="eafe3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eafe3-107">Permissions</span></span>
<span data-ttu-id="eafe3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eafe3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eafe3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eafe3-110">Permission type</span></span>      | <span data-ttu-id="eafe3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eafe3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eafe3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eafe3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eafe3-113">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eafe3-113">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eafe3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eafe3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eafe3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eafe3-115">Not supported.</span></span>    |
|<span data-ttu-id="eafe3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eafe3-116">Application</span></span> | <span data-ttu-id="eafe3-117">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eafe3-117">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eafe3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eafe3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="eafe3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eafe3-119">Request headers</span></span>
| <span data-ttu-id="eafe3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eafe3-120">Header</span></span>       | <span data-ttu-id="eafe3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eafe3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eafe3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eafe3-122">Authorization</span></span>  | <span data-ttu-id="eafe3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eafe3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eafe3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eafe3-125">Content-Type</span></span>  | <span data-ttu-id="eafe3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eafe3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eafe3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eafe3-127">Request body</span></span>
<span data-ttu-id="eafe3-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="eafe3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eafe3-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="eafe3-129">Parameter</span></span>    | <span data-ttu-id="eafe3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eafe3-130">Type</span></span>   |<span data-ttu-id="eafe3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eafe3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eafe3-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="eafe3-132">securityEnabledOnly</span></span>|<span data-ttu-id="eafe3-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="eafe3-133">Boolean</span></span>|<span data-ttu-id="eafe3-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является пользователь. Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eafe3-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="eafe3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafe3-136">Response</span></span>

<span data-ttu-id="eafe3-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="eafe3-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="eafe3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="eafe3-138">Example</span></span>
<span data-ttu-id="eafe3-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="eafe3-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eafe3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="eafe3-140">Request</span></span>
<span data-ttu-id="eafe3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eafe3-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eafe3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="eafe3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="eafe3-143">C#</span><span class="sxs-lookup"><span data-stu-id="eafe3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eafe3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eafe3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eafe3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eafe3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eafe3-146">Java</span><span class="sxs-lookup"><span data-stu-id="eafe3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eafe3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafe3-147">Response</span></span>
<span data-ttu-id="eafe3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eafe3-148">Here is an example of the response.</span></span> <span data-ttu-id="eafe3-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eafe3-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

