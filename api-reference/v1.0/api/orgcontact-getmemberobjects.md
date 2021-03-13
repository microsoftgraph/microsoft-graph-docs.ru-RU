---
title: 'orgContact: getMemberObjects'
description: Верни все группы, в которые входит этот организационный контакт. Это транзитивная проверка.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a51cd565b363e1fe080f5a1d48de9f51b38d78f7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761641"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="dd004-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="dd004-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="dd004-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd004-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd004-106">Верни все группы, в [которые](../resources/orgcontact.md) входит этот организационный контакт.</span><span class="sxs-lookup"><span data-stu-id="dd004-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="dd004-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="dd004-107">The check is transitive.</span></span> <span data-ttu-id="dd004-108">Организационные контакты не могут быть членами ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="dd004-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="dd004-109">Роли каталога не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="dd004-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd004-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd004-110">Permissions</span></span>
<span data-ttu-id="dd004-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd004-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd004-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd004-113">Permission type</span></span>      | <span data-ttu-id="dd004-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd004-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd004-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd004-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dd004-116">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd004-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="dd004-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd004-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd004-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd004-118">Not supported.</span></span>    |
|<span data-ttu-id="dd004-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd004-119">Application</span></span> | <span data-ttu-id="dd004-120">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd004-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd004-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd004-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="dd004-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd004-122">Request headers</span></span>
| <span data-ttu-id="dd004-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd004-123">Header</span></span>       | <span data-ttu-id="dd004-124">Значение</span><span class="sxs-lookup"><span data-stu-id="dd004-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="dd004-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd004-125">Authorization</span></span>  | <span data-ttu-id="dd004-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd004-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd004-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd004-128">Content-type</span></span>   | <span data-ttu-id="dd004-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd004-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd004-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd004-131">Request body</span></span>
<span data-ttu-id="dd004-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dd004-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd004-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd004-133">Parameter</span></span>    | <span data-ttu-id="dd004-134">Тип</span><span class="sxs-lookup"><span data-stu-id="dd004-134">Type</span></span>   |<span data-ttu-id="dd004-135">Описание</span><span class="sxs-lookup"><span data-stu-id="dd004-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd004-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dd004-136">securityEnabledOnly</span></span>|<span data-ttu-id="dd004-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd004-137">Boolean</span></span>|<span data-ttu-id="dd004-138">Установите `false` для .</span><span class="sxs-lookup"><span data-stu-id="dd004-138">Set to `false`.</span></span> <span data-ttu-id="dd004-139">Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd004-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="dd004-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd004-140">Response</span></span>

<span data-ttu-id="dd004-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd004-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd004-142">Пример</span><span class="sxs-lookup"><span data-stu-id="dd004-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd004-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd004-143">Request</span></span>
<span data-ttu-id="dd004-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd004-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd004-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd004-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="dd004-146">C#</span><span class="sxs-lookup"><span data-stu-id="dd004-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd004-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd004-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd004-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd004-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd004-149">Java</span><span class="sxs-lookup"><span data-stu-id="dd004-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd004-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd004-150">Response</span></span>
<span data-ttu-id="dd004-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd004-151">The following is an example of the response.</span></span>
><span data-ttu-id="dd004-152">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd004-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

