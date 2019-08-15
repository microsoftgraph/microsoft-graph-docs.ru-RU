---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4fee17b7f01299c6f35eb056fb1a8bc8b4ce4a85
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409172"
---
# <a name="checkmembergroups"></a><span data-ttu-id="594f8-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="594f8-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="594f8-p102">Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="594f8-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="594f8-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, участие в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="594f8-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="594f8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="594f8-111">Permissions</span></span>

<span data-ttu-id="594f8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="594f8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="594f8-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="594f8-114">Permission type</span></span>                        | <span data-ttu-id="594f8-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="594f8-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="594f8-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="594f8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="594f8-117">User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, User. ReadWrite. ALL и Group. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="594f8-117">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="594f8-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="594f8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="594f8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="594f8-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="594f8-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="594f8-120">Application</span></span>                            | <span data-ttu-id="594f8-121">User. Read. ALL и Group. Read. ALL, User. ReadWrite. ALL и Group. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="594f8-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="594f8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="594f8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="594f8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="594f8-123">Request headers</span></span>

| <span data-ttu-id="594f8-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="594f8-124">Header</span></span>        | <span data-ttu-id="594f8-125">Значение</span><span class="sxs-lookup"><span data-stu-id="594f8-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="594f8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="594f8-126">Authorization</span></span> | <span data-ttu-id="594f8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="594f8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="594f8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="594f8-129">Content-Type</span></span>  | <span data-ttu-id="594f8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="594f8-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="594f8-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="594f8-131">Request body</span></span>

<span data-ttu-id="594f8-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="594f8-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="594f8-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="594f8-133">Parameter</span></span> | <span data-ttu-id="594f8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="594f8-134">Type</span></span>   | <span data-ttu-id="594f8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="594f8-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="594f8-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="594f8-136">groupIds</span></span>  | <span data-ttu-id="594f8-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="594f8-137">String collection</span></span> | <span data-ttu-id="594f8-138">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="594f8-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="594f8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="594f8-139">Response</span></span>

<span data-ttu-id="594f8-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="594f8-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="594f8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="594f8-141">Example</span></span>

<span data-ttu-id="594f8-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="594f8-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="594f8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="594f8-143">Request</span></span>

<span data-ttu-id="594f8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="594f8-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="594f8-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="594f8-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="594f8-146">C#</span><span class="sxs-lookup"><span data-stu-id="594f8-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="594f8-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="594f8-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="594f8-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="594f8-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="594f8-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="594f8-149">Response</span></span>

<span data-ttu-id="594f8-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="594f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
