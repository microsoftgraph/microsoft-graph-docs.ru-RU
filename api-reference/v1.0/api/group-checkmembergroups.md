---
title: 'group: checkMemberGroups'
description: Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 0c0b850857b094567ba04c8c701227a6dda742bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275882"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="ea7eb-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ea7eb-104">group: checkMemberGroups</span></span>

<span data-ttu-id="ea7eb-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="ea7eb-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea7eb-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7eb-111">Permissions</span></span>

<span data-ttu-id="ea7eb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea7eb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea7eb-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7eb-114">Permission type</span></span>                        | <span data-ttu-id="ea7eb-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea7eb-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="ea7eb-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea7eb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea7eb-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea7eb-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ea7eb-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea7eb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea7eb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="ea7eb-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea7eb-120">Application</span></span>                            | <span data-ttu-id="ea7eb-121">_Group.Read.All_, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea7eb-121">_Group.Read.All_, Directory.Read.All.</span></span> <span data-ttu-id="ea7eb-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7eb-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="ea7eb-123">**Примечание.** В настоящее время для вызова этого API требуется разрешение `Directory.Read.All` или выше.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-123">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="ea7eb-124">При использовании разрешения `Group.Read.All` возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-124">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="ea7eb-125">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="ea7eb-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea7eb-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="ea7eb-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea7eb-127">Request headers</span></span>

| <span data-ttu-id="ea7eb-128">Имя</span><span class="sxs-lookup"><span data-stu-id="ea7eb-128">Name</span></span>          | <span data-ttu-id="ea7eb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ea7eb-129">Type</span></span>   | <span data-ttu-id="ea7eb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ea7eb-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="ea7eb-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea7eb-131">Authorization</span></span> | <span data-ttu-id="ea7eb-132">string</span><span class="sxs-lookup"><span data-stu-id="ea7eb-132">string</span></span> | <span data-ttu-id="ea7eb-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea7eb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea7eb-135">Request body</span></span>

<span data-ttu-id="ea7eb-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea7eb-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="ea7eb-137">Parameter</span></span> | <span data-ttu-id="ea7eb-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ea7eb-138">Type</span></span>              | <span data-ttu-id="ea7eb-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ea7eb-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="ea7eb-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="ea7eb-140">groupIds</span></span>  | <span data-ttu-id="ea7eb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea7eb-141">String collection</span></span> | <span data-ttu-id="ea7eb-142">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="ea7eb-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="ea7eb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea7eb-143">Response</span></span>

<span data-ttu-id="ea7eb-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7eb-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ea7eb-145">Example</span></span>

<span data-ttu-id="ea7eb-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ea7eb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea7eb-147">Request</span></span>

<span data-ttu-id="ea7eb-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-148">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="ea7eb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea7eb-149">Response</span></span>

<span data-ttu-id="ea7eb-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea7eb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ea7eb-153">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ea7eb-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ea7eb-154">C#</span><span class="sxs-lookup"><span data-stu-id="ea7eb-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea7eb-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea7eb-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ea7eb-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea7eb-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
