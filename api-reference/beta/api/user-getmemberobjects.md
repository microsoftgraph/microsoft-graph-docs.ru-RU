---
title: 'user: getMemberObjects'
description: Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d5ea5ef17550f5f821f85c8e38a341075639f297
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970290"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="6d5f2-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="6d5f2-104">user: getMemberObjects</span></span>

<span data-ttu-id="6d5f2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d5f2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d5f2-p102">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d5f2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d5f2-108">Permissions</span></span>
<span data-ttu-id="6d5f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d5f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6d5f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d5f2-111">Permission type</span></span>      | <span data-ttu-id="6d5f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d5f2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d5f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d5f2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6d5f2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d5f2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d5f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d5f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d5f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-116">Not supported.</span></span>    |
|<span data-ttu-id="6d5f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d5f2-117">Application</span></span> | <span data-ttu-id="6d5f2-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d5f2-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d5f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d5f2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="6d5f2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d5f2-120">Request headers</span></span>
| <span data-ttu-id="6d5f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d5f2-121">Header</span></span>       | <span data-ttu-id="6d5f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d5f2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d5f2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d5f2-123">Authorization</span></span>  | <span data-ttu-id="6d5f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d5f2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d5f2-126">Content-Type</span></span>  | <span data-ttu-id="6d5f2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6d5f2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d5f2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d5f2-128">Request body</span></span>
<span data-ttu-id="6d5f2-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d5f2-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d5f2-130">Parameter</span></span>    | <span data-ttu-id="6d5f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d5f2-131">Type</span></span>   |<span data-ttu-id="6d5f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d5f2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d5f2-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6d5f2-133">securityEnabledOnly</span></span>|<span data-ttu-id="6d5f2-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d5f2-134">Boolean</span></span>|<span data-ttu-id="6d5f2-p105">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="6d5f2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d5f2-137">Response</span></span>

<span data-ttu-id="6d5f2-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="6d5f2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6d5f2-139">Example</span></span>
<span data-ttu-id="6d5f2-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6d5f2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d5f2-141">Request</span></span>
<span data-ttu-id="6d5f2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d5f2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d5f2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="6d5f2-144">C#</span><span class="sxs-lookup"><span data-stu-id="6d5f2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d5f2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d5f2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d5f2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d5f2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d5f2-147">Java</span><span class="sxs-lookup"><span data-stu-id="6d5f2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d5f2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d5f2-148">Response</span></span>
<span data-ttu-id="6d5f2-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d5f2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


