---
title: 'orgContact: getMemberObjects'
description: Возврат всех групп, членом которых является это организационное Контактное лицо. Это транзитивная проверка.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b28bb43ae8b37a7a7007b725bb6e788d052ed29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511189"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="4b5ca-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4b5ca-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="4b5ca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b5ca-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b5ca-106">Возврат всех групп, членом которых является это [организационное Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="4b5ca-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="4b5ca-107">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-107">The check is transitive.</span></span> <span data-ttu-id="4b5ca-108">Организационные контакты не могут быть членами ролей каталогов.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="4b5ca-109">Роли каталога не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b5ca-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b5ca-110">Permissions</span></span>
<span data-ttu-id="4b5ca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b5ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5ca-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b5ca-113">Permission type</span></span>      | <span data-ttu-id="4b5ca-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b5ca-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b5ca-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b5ca-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4b5ca-116">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4b5ca-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="4b5ca-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b5ca-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b5ca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-118">Not supported.</span></span>    |
|<span data-ttu-id="4b5ca-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b5ca-119">Application</span></span> | <span data-ttu-id="4b5ca-120">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4b5ca-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b5ca-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b5ca-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="4b5ca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b5ca-122">Request headers</span></span>
| <span data-ttu-id="4b5ca-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b5ca-123">Header</span></span>       | <span data-ttu-id="4b5ca-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4b5ca-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4b5ca-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b5ca-125">Authorization</span></span>  | <span data-ttu-id="4b5ca-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b5ca-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b5ca-128">Content-type</span></span>   | <span data-ttu-id="4b5ca-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5ca-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b5ca-131">Request body</span></span>
<span data-ttu-id="4b5ca-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b5ca-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b5ca-133">Parameter</span></span>    | <span data-ttu-id="4b5ca-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4b5ca-134">Type</span></span>   |<span data-ttu-id="4b5ca-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4b5ca-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b5ca-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4b5ca-136">securityEnabledOnly</span></span>|<span data-ttu-id="4b5ca-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="4b5ca-137">Boolean</span></span>|<span data-ttu-id="4b5ca-138">Значение `false`.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-138">Set to `false`.</span></span> <span data-ttu-id="4b5ca-139">Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="4b5ca-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5ca-140">Response</span></span>

<span data-ttu-id="4b5ca-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5ca-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4b5ca-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4b5ca-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b5ca-143">Request</span></span>
<span data-ttu-id="4b5ca-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b5ca-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b5ca-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4b5ca-146">C#</span><span class="sxs-lookup"><span data-stu-id="4b5ca-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b5ca-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b5ca-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b5ca-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b5ca-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b5ca-149">Java</span><span class="sxs-lookup"><span data-stu-id="4b5ca-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4b5ca-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5ca-150">Response</span></span>
<span data-ttu-id="4b5ca-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-151">The following is an example of the response.</span></span>
><span data-ttu-id="4b5ca-152">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b5ca-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
