---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8c0c56f83a2a420a88590f36ab4de5f3942e334b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976617"
---
# <a name="checkmembergroups"></a><span data-ttu-id="78779-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="78779-104">checkMemberGroups</span></span>

<span data-ttu-id="78779-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78779-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78779-p102">Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="78779-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="78779-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Microsoft 365 не могут содержать групп. Следовательно, участие в группе Microsoft 365 всегда является прямым.</span><span class="sxs-lookup"><span data-stu-id="78779-p103">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="78779-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78779-112">Permissions</span></span>

<span data-ttu-id="78779-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78779-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78779-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78779-115">Permission type</span></span>                        | <span data-ttu-id="78779-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78779-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="78779-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78779-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="78779-118">User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, User.ReadWrite.All и GroupMember.Read.All, User.ReadWrite.All и Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="78779-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="78779-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78779-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78779-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78779-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="78779-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="78779-121">Application</span></span>                            | <span data-ttu-id="78779-122">User. Read. ALL и Граупмембер. Read. ALL, User. Read. ALL и Group. Read. ALL, User. ReadWrite. ALL и Граупмембер. Read. ALL, User. ReadWrite. ALL и Group. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="78779-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78779-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78779-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="78779-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78779-124">Request headers</span></span>

| <span data-ttu-id="78779-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78779-125">Header</span></span>        | <span data-ttu-id="78779-126">Значение</span><span class="sxs-lookup"><span data-stu-id="78779-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="78779-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78779-127">Authorization</span></span> | <span data-ttu-id="78779-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78779-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78779-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78779-130">Content-Type</span></span>  | <span data-ttu-id="78779-131">application/json</span><span class="sxs-lookup"><span data-stu-id="78779-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="78779-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78779-132">Request body</span></span>

<span data-ttu-id="78779-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="78779-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78779-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="78779-134">Parameter</span></span> | <span data-ttu-id="78779-135">Тип</span><span class="sxs-lookup"><span data-stu-id="78779-135">Type</span></span>   | <span data-ttu-id="78779-136">Описание</span><span class="sxs-lookup"><span data-stu-id="78779-136">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="78779-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="78779-137">groupIds</span></span>  | <span data-ttu-id="78779-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="78779-138">String collection</span></span> | <span data-ttu-id="78779-139">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="78779-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="78779-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="78779-140">Response</span></span>

<span data-ttu-id="78779-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78779-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78779-142">Пример</span><span class="sxs-lookup"><span data-stu-id="78779-142">Example</span></span>

<span data-ttu-id="78779-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="78779-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="78779-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="78779-144">Request</span></span>

<span data-ttu-id="78779-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78779-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="78779-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="78779-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="78779-147">C#</span><span class="sxs-lookup"><span data-stu-id="78779-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78779-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78779-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78779-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78779-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78779-150">Java</span><span class="sxs-lookup"><span data-stu-id="78779-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78779-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="78779-151">Response</span></span>

<span data-ttu-id="78779-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78779-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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


