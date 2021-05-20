---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: yyuank
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: faa5ecf8609e4807614a66faa9cf56e9d51fbb83
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547592"
---
# <a name="checkmembergroups"></a><span data-ttu-id="9ebb8-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9ebb8-104">checkMemberGroups</span></span>

<span data-ttu-id="9ebb8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ebb8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ebb8-p102">Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="9ebb8-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Microsoft 365 не могут содержать групп. Следовательно, участие в группе Microsoft 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-p103">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ebb8-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ebb8-112">Permissions</span></span>

<span data-ttu-id="9ebb8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ebb8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ebb8-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ebb8-115">Permission type</span></span>                        | <span data-ttu-id="9ebb8-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ebb8-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9ebb8-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ebb8-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ebb8-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ebb8-118">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9ebb8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ebb8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ebb8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="9ebb8-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ebb8-121">Application</span></span>                            | <span data-ttu-id="9ebb8-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ebb8-122">User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ebb8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ebb8-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9ebb8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ebb8-124">Request headers</span></span>

| <span data-ttu-id="9ebb8-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ebb8-125">Header</span></span>        | <span data-ttu-id="9ebb8-126">Значение</span><span class="sxs-lookup"><span data-stu-id="9ebb8-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9ebb8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ebb8-127">Authorization</span></span> | <span data-ttu-id="9ebb8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ebb8-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ebb8-130">Content-Type</span></span>  | <span data-ttu-id="9ebb8-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9ebb8-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9ebb8-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ebb8-132">Request body</span></span>

<span data-ttu-id="9ebb8-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ebb8-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ebb8-134">Parameter</span></span> | <span data-ttu-id="9ebb8-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9ebb8-135">Type</span></span>              | <span data-ttu-id="9ebb8-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9ebb8-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="9ebb8-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="9ebb8-137">groupIds</span></span>  | <span data-ttu-id="9ebb8-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ebb8-138">String collection</span></span> | <span data-ttu-id="9ebb8-139">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="9ebb8-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="9ebb8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ebb8-140">Response</span></span>

<span data-ttu-id="9ebb8-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ebb8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9ebb8-142">Example</span></span>

<span data-ttu-id="9ebb8-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9ebb8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ebb8-144">Request</span></span>

<span data-ttu-id="9ebb8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ebb8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ebb8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9ebb8-147">C#</span><span class="sxs-lookup"><span data-stu-id="9ebb8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ebb8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ebb8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ebb8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ebb8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ebb8-150">Java</span><span class="sxs-lookup"><span data-stu-id="9ebb8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ebb8-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ebb8-151">Response</span></span>

<span data-ttu-id="9ebb8-p106">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ebb8-p106">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

