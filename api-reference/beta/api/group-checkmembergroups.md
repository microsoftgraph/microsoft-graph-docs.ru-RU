---
title: 'group: checkMemberGroups'
description: Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8d9219050cce3e633509d44e5d0c1d57eafbc98c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859023"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="276bf-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="276bf-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="276bf-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="276bf-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="276bf-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="276bf-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="276bf-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="276bf-111">Permissions</span></span>

<span data-ttu-id="276bf-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="276bf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="276bf-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="276bf-114">Permission type</span></span>                        | <span data-ttu-id="276bf-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="276bf-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="276bf-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="276bf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="276bf-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="276bf-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="276bf-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="276bf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276bf-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="276bf-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="276bf-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="276bf-120">Application</span></span>                            | <span data-ttu-id="276bf-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="276bf-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="276bf-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="276bf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="276bf-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="276bf-123">Request headers</span></span>

| <span data-ttu-id="276bf-124">Имя</span><span class="sxs-lookup"><span data-stu-id="276bf-124">Name</span></span>          | <span data-ttu-id="276bf-125">Тип</span><span class="sxs-lookup"><span data-stu-id="276bf-125">Type</span></span>   | <span data-ttu-id="276bf-126">Описание</span><span class="sxs-lookup"><span data-stu-id="276bf-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="276bf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="276bf-127">Authorization</span></span> | <span data-ttu-id="276bf-128">string</span><span class="sxs-lookup"><span data-stu-id="276bf-128">string</span></span> | <span data-ttu-id="276bf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="276bf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="276bf-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="276bf-131">Request body</span></span>

<span data-ttu-id="276bf-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="276bf-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="276bf-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="276bf-133">Parameter</span></span> | <span data-ttu-id="276bf-134">Тип</span><span class="sxs-lookup"><span data-stu-id="276bf-134">Type</span></span>   | <span data-ttu-id="276bf-135">Описание</span><span class="sxs-lookup"><span data-stu-id="276bf-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="276bf-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="276bf-136">groupIds</span></span>  | <span data-ttu-id="276bf-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="276bf-137">String collection</span></span> | <span data-ttu-id="276bf-138">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="276bf-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="276bf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="276bf-139">Response</span></span>

<span data-ttu-id="276bf-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="276bf-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="276bf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="276bf-141">Example</span></span>

<span data-ttu-id="276bf-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="276bf-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="276bf-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="276bf-143">Request</span></span>

<span data-ttu-id="276bf-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="276bf-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="276bf-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="276bf-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="276bf-146">C#</span><span class="sxs-lookup"><span data-stu-id="276bf-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="276bf-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="276bf-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="276bf-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="276bf-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="276bf-149">Java</span><span class="sxs-lookup"><span data-stu-id="276bf-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="276bf-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="276bf-150">Response</span></span>

<span data-ttu-id="276bf-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="276bf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
