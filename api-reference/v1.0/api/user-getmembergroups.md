---
title: 'user: getMemberGroups'
description: Возвращает все группы, в которых состоит пользователь. Это промежуточная проверка, в отличие от считывания
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a28a32ce1af781ea2d6eb05e18240067562c179a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055682"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="bc185-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bc185-104">user: getMemberGroups</span></span>

<span data-ttu-id="bc185-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc185-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc185-p102">Возвращение всех названий групп, в которых состоит пользователь. Проверка промежуточная, в отличие от считывания свойства навигации [memberOf](../api/user-list-memberof.md) (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="bc185-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="bc185-p103">Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос — 2046. Обратите внимание, что компонент "Группы Microsoft 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Microsoft 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="bc185-p103">This function supports Microsoft 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc185-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc185-112">Permissions</span></span>

<span data-ttu-id="bc185-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc185-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc185-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc185-115">Permission type</span></span>                        | <span data-ttu-id="bc185-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc185-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bc185-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc185-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc185-118">User.ReadBasic.All, User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc185-118">User.ReadBasic.All, User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="bc185-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc185-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc185-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc185-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="bc185-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc185-121">Application</span></span>                            |  <span data-ttu-id="bc185-122">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc185-122">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc185-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc185-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="bc185-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc185-124">Request headers</span></span>

| <span data-ttu-id="bc185-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc185-125">Header</span></span>        | <span data-ttu-id="bc185-126">Значение</span><span class="sxs-lookup"><span data-stu-id="bc185-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="bc185-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc185-127">Authorization</span></span> | <span data-ttu-id="bc185-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc185-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc185-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc185-130">Content-Type</span></span>  | <span data-ttu-id="bc185-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bc185-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="bc185-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc185-132">Request body</span></span>

<span data-ttu-id="bc185-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bc185-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc185-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="bc185-134">Parameter</span></span>           | <span data-ttu-id="bc185-135">Тип</span><span class="sxs-lookup"><span data-stu-id="bc185-135">Type</span></span>    | <span data-ttu-id="bc185-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bc185-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bc185-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="bc185-137">securityEnabledOnly</span></span> | <span data-ttu-id="bc185-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="bc185-138">Boolean</span></span> | <span data-ttu-id="bc185-p106">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc185-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="bc185-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc185-141">Response</span></span>

<span data-ttu-id="bc185-142">В случае успеха этот метод возвратит код отклика `200 OK` и коллекцию String в теле отклика, которое содержит идентификаторы групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="bc185-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="bc185-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bc185-143">Example</span></span>

<span data-ttu-id="bc185-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bc185-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bc185-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc185-145">Request</span></span>

<span data-ttu-id="bc185-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc185-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc185-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc185-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="bc185-148">C#</span><span class="sxs-lookup"><span data-stu-id="bc185-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc185-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc185-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc185-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc185-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc185-151">Java</span><span class="sxs-lookup"><span data-stu-id="bc185-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bc185-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc185-152">Response</span></span>

<span data-ttu-id="bc185-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc185-153">Here is an example of the response.</span></span> <span data-ttu-id="bc185-154">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bc185-154">Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

