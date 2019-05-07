---
title: 'user: getMemberGroups'
description: 'Возвращает все группы, в которых состоит пользователь. Это промежуточная проверка, в отличие от считывания '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9b508998f3dbd24e66afdfcccd3156ebfcf668cd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637327"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="d1407-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d1407-104">user: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1407-p102">Возвращение всех названий групп, в которых состоит пользователь. Проверка промежуточная, в отличие от считывания свойства навигации [memberOf](../api/user-list-memberof.md) (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="d1407-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="d1407-p103">Эта функция поддерживает Office 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос, — 2046. Обратите внимание, что компонент "Группы Office 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Office 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="d1407-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1407-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1407-111">Permissions</span></span>

<span data-ttu-id="d1407-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1407-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1407-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1407-114">Permission type</span></span>                        | <span data-ttu-id="d1407-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1407-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d1407-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1407-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1407-117">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1407-117">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d1407-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1407-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1407-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1407-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="d1407-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1407-120">Application</span></span>                            | <span data-ttu-id="d1407-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1407-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

## <a name="http-request"></a><span data-ttu-id="d1407-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1407-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d1407-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1407-123">Request headers</span></span>

| <span data-ttu-id="d1407-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1407-124">Header</span></span>        | <span data-ttu-id="d1407-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d1407-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d1407-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1407-126">Authorization</span></span> | <span data-ttu-id="d1407-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1407-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1407-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1407-129">Content-Type</span></span>  | <span data-ttu-id="d1407-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d1407-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d1407-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1407-131">Request body</span></span>

<span data-ttu-id="d1407-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d1407-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1407-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1407-133">Parameter</span></span>           | <span data-ttu-id="d1407-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d1407-134">Type</span></span>    | <span data-ttu-id="d1407-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d1407-135">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d1407-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d1407-136">securityEnabledOnly</span></span> | <span data-ttu-id="d1407-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="d1407-137">Boolean</span></span> | <span data-ttu-id="d1407-p106">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1407-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="d1407-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1407-140">Response</span></span>

<span data-ttu-id="d1407-141">В случае успеха этот метод возвратит код отклика `200 OK` и коллекцию String в теле отклика, которое содержит идентификаторы групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="d1407-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="d1407-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d1407-142">Example</span></span>

<span data-ttu-id="d1407-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1407-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d1407-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1407-144">Request</span></span>

<span data-ttu-id="d1407-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1407-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="d1407-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1407-146">Response</span></span>

<span data-ttu-id="d1407-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1407-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1407-150">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d1407-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1407-151">Языках</span><span class="sxs-lookup"><span data-stu-id="d1407-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1407-152">Язык</span><span class="sxs-lookup"><span data-stu-id="d1407-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_getmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
