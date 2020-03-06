---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30338b63b8a60865049c74c2ab26105ac7f56c00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509239"
---
# <a name="checkmembergroups"></a><span data-ttu-id="23cbf-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="23cbf-104">checkMemberGroups</span></span>

<span data-ttu-id="23cbf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23cbf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23cbf-p102">Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="23cbf-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="23cbf-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, участие в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="23cbf-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="23cbf-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23cbf-112">Permissions</span></span>

<span data-ttu-id="23cbf-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cbf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23cbf-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23cbf-115">Permission type</span></span>                        | <span data-ttu-id="23cbf-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23cbf-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="23cbf-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23cbf-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="23cbf-118">User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, User.ReadWrite.All и GroupMember.Read.All, User.ReadWrite.All и Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23cbf-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="23cbf-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23cbf-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23cbf-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbf-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="23cbf-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="23cbf-121">Application</span></span>                            | <span data-ttu-id="23cbf-122">User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, User.ReadWrite.All и GroupMember.Read.All User.ReadWrite.All и Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cbf-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23cbf-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23cbf-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="23cbf-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23cbf-124">Request headers</span></span>

| <span data-ttu-id="23cbf-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23cbf-125">Header</span></span>        | <span data-ttu-id="23cbf-126">Значение</span><span class="sxs-lookup"><span data-stu-id="23cbf-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="23cbf-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23cbf-127">Authorization</span></span> | <span data-ttu-id="23cbf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23cbf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23cbf-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23cbf-130">Content-Type</span></span>  | <span data-ttu-id="23cbf-131">application/json</span><span class="sxs-lookup"><span data-stu-id="23cbf-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="23cbf-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23cbf-132">Request body</span></span>

<span data-ttu-id="23cbf-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="23cbf-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23cbf-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="23cbf-134">Parameter</span></span> | <span data-ttu-id="23cbf-135">Тип</span><span class="sxs-lookup"><span data-stu-id="23cbf-135">Type</span></span>              | <span data-ttu-id="23cbf-136">Описание</span><span class="sxs-lookup"><span data-stu-id="23cbf-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="23cbf-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="23cbf-137">groupIds</span></span>  | <span data-ttu-id="23cbf-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23cbf-138">String collection</span></span> | <span data-ttu-id="23cbf-139">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="23cbf-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="23cbf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbf-140">Response</span></span>

<span data-ttu-id="23cbf-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23cbf-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cbf-142">Пример</span><span class="sxs-lookup"><span data-stu-id="23cbf-142">Example</span></span>

<span data-ttu-id="23cbf-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="23cbf-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="23cbf-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="23cbf-144">Request</span></span>

<span data-ttu-id="23cbf-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23cbf-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23cbf-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="23cbf-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="23cbf-147">C#</span><span class="sxs-lookup"><span data-stu-id="23cbf-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23cbf-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23cbf-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23cbf-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23cbf-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23cbf-150">Java</span><span class="sxs-lookup"><span data-stu-id="23cbf-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23cbf-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbf-151">Response</span></span>

<span data-ttu-id="23cbf-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23cbf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
