---
title: 'group: getMemberGroups'
description: Возвращение всех групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации memberOf (возвращаются только группы, непосредственным участником которых является данная группа).
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8a3b2fa52ff12b30e431c5dc925dffd6090b31ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273558"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="9d9e1-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9d9e1-104">group: getMemberGroups</span></span>

<span data-ttu-id="9d9e1-p102">Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации [memberOf](../api/group-list-memberof.md) (возвращаются только группы, непосредственным членом которых является данная группа).</span><span class="sxs-lookup"><span data-stu-id="9d9e1-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="9d9e1-p103">Эта функция поддерживает Office 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос, — 2046. Обратите внимание, что компонент "Группы Office 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Office 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d9e1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d9e1-111">Permissions</span></span>

<span data-ttu-id="9d9e1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d9e1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d9e1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d9e1-114">Permission type</span></span>                        | <span data-ttu-id="9d9e1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d9e1-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9d9e1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d9e1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d9e1-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d9e1-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9d9e1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d9e1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d9e1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="9d9e1-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d9e1-120">Application</span></span>                            | <span data-ttu-id="9d9e1-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d9e1-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |


## <a name="http-request"></a><span data-ttu-id="9d9e1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d9e1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9d9e1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d9e1-123">Request headers</span></span>

| <span data-ttu-id="9d9e1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9d9e1-124">Name</span></span>          | <span data-ttu-id="9d9e1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9d9e1-125">Type</span></span>   | <span data-ttu-id="9d9e1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9e1-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="9d9e1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d9e1-127">Authorization</span></span> | <span data-ttu-id="9d9e1-128">string</span><span class="sxs-lookup"><span data-stu-id="9d9e1-128">string</span></span> | <span data-ttu-id="9d9e1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d9e1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d9e1-131">Request body</span></span>

<span data-ttu-id="9d9e1-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d9e1-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="9d9e1-133">Parameter</span></span>           | <span data-ttu-id="9d9e1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9d9e1-134">Type</span></span>    | <span data-ttu-id="9d9e1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9e1-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="9d9e1-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9d9e1-136">securityEnabledOnly</span></span> | <span data-ttu-id="9d9e1-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="9d9e1-137">Boolean</span></span> | <span data-ttu-id="9d9e1-p106">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="9d9e1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d9e1-140">Response</span></span>

<span data-ttu-id="9d9e1-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="9d9e1-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9d9e1-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9d9e1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d9e1-143">Request</span></span>

<span data-ttu-id="9d9e1-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="9d9e1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d9e1-145">Response</span></span>

<span data-ttu-id="9d9e1-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-146">The following is an example of the response.</span></span>

> <span data-ttu-id="9d9e1-147">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9d9e1-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d9e1-148">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9d9e1-149">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="9d9e1-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9d9e1-150">C#</span><span class="sxs-lookup"><span data-stu-id="9d9e1-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d9e1-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d9e1-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9d9e1-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d9e1-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_getmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
