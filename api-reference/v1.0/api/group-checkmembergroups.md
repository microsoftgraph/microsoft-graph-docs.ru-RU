---
title: 'group: checkMemberGroups'
description: Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ad182a184455872b961af8f1df825774e29009db
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448147"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="36d12-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="36d12-104">group: checkMemberGroups</span></span>

<span data-ttu-id="36d12-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="36d12-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="36d12-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="36d12-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="36d12-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36d12-111">Permissions</span></span>

<span data-ttu-id="36d12-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36d12-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36d12-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36d12-114">Permission type</span></span>                        | <span data-ttu-id="36d12-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36d12-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="36d12-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36d12-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="36d12-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36d12-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="36d12-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36d12-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36d12-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d12-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="36d12-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="36d12-120">Application</span></span>                            | <span data-ttu-id="36d12-121">Group.Read.All, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="36d12-121">Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="36d12-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36d12-122">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="36d12-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36d12-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="36d12-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36d12-124">Request headers</span></span>

| <span data-ttu-id="36d12-125">Имя</span><span class="sxs-lookup"><span data-stu-id="36d12-125">Name</span></span>          | <span data-ttu-id="36d12-126">Тип</span><span class="sxs-lookup"><span data-stu-id="36d12-126">Type</span></span>   | <span data-ttu-id="36d12-127">Описание</span><span class="sxs-lookup"><span data-stu-id="36d12-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="36d12-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="36d12-128">Authorization</span></span> | <span data-ttu-id="36d12-129">string</span><span class="sxs-lookup"><span data-stu-id="36d12-129">string</span></span> | <span data-ttu-id="36d12-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36d12-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36d12-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36d12-132">Request body</span></span>

<span data-ttu-id="36d12-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="36d12-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="36d12-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="36d12-134">Parameter</span></span> | <span data-ttu-id="36d12-135">Тип</span><span class="sxs-lookup"><span data-stu-id="36d12-135">Type</span></span>              | <span data-ttu-id="36d12-136">Описание</span><span class="sxs-lookup"><span data-stu-id="36d12-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="36d12-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="36d12-137">groupIds</span></span>  | <span data-ttu-id="36d12-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36d12-138">String collection</span></span> | <span data-ttu-id="36d12-139">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="36d12-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="36d12-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="36d12-140">Response</span></span>

<span data-ttu-id="36d12-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36d12-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d12-142">Пример</span><span class="sxs-lookup"><span data-stu-id="36d12-142">Example</span></span>

<span data-ttu-id="36d12-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="36d12-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="36d12-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="36d12-144">Request</span></span>

<span data-ttu-id="36d12-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36d12-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36d12-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="36d12-146">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="36d12-147">C#</span><span class="sxs-lookup"><span data-stu-id="36d12-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36d12-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36d12-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36d12-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36d12-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36d12-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="36d12-150">Response</span></span>

<span data-ttu-id="36d12-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36d12-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
