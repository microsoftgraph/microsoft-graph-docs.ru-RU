---
title: 'group: checkMemberGroups'
description: Проверка участия в указанном списке групп.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f6fd1c019a9141ba343ca770ee28cf82d60fce3c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052371"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="263d1-103">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="263d1-103">group: checkMemberGroups</span></span>

<span data-ttu-id="263d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="263d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="263d1-p101">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="263d1-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="263d1-p102">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Microsoft 365 не могут содержать группы. Следовательно, участие в группе Microsoft 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="263d1-p102">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="263d1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="263d1-111">Permissions</span></span>

<span data-ttu-id="263d1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="263d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="263d1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="263d1-114">Permission type</span></span>                        | <span data-ttu-id="263d1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="263d1-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="263d1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="263d1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="263d1-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="263d1-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="263d1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="263d1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="263d1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="263d1-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="263d1-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="263d1-120">Application</span></span>                            | <span data-ttu-id="263d1-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263d1-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="263d1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="263d1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="263d1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="263d1-123">Request headers</span></span>

| <span data-ttu-id="263d1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="263d1-124">Name</span></span>          | <span data-ttu-id="263d1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="263d1-125">Type</span></span>   | <span data-ttu-id="263d1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="263d1-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="263d1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="263d1-127">Authorization</span></span> | <span data-ttu-id="263d1-128">string</span><span class="sxs-lookup"><span data-stu-id="263d1-128">string</span></span> | <span data-ttu-id="263d1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="263d1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="263d1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="263d1-131">Request body</span></span>

<span data-ttu-id="263d1-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="263d1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="263d1-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="263d1-133">Parameter</span></span> | <span data-ttu-id="263d1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="263d1-134">Type</span></span>              | <span data-ttu-id="263d1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="263d1-135">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="263d1-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="263d1-136">groupIds</span></span>  | <span data-ttu-id="263d1-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="263d1-137">String collection</span></span> | <span data-ttu-id="263d1-138">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="263d1-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="263d1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="263d1-139">Response</span></span>

<span data-ttu-id="263d1-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="263d1-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263d1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="263d1-141">Example</span></span>

<span data-ttu-id="263d1-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="263d1-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="263d1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="263d1-143">Request</span></span>

<span data-ttu-id="263d1-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="263d1-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="263d1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="263d1-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="263d1-146">C#</span><span class="sxs-lookup"><span data-stu-id="263d1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="263d1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="263d1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="263d1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="263d1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="263d1-149">Java</span><span class="sxs-lookup"><span data-stu-id="263d1-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="263d1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="263d1-150">Response</span></span>

<span data-ttu-id="263d1-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="263d1-151">Here is an example of the response.</span></span> <span data-ttu-id="263d1-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="263d1-152">Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

