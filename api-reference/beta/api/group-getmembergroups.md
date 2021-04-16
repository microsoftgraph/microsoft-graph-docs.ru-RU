---
title: 'group: getMemberGroups'
description: Возвращение всех групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации memberOf (возвращаются только группы, непосредственным участником которых является данная группа).
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0d26366b9a9ba553abf9e8bb559b0f5eefe03ac8
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869759"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="d7644-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d7644-104">group: getMemberGroups</span></span>

<span data-ttu-id="d7644-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7644-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7644-p102">Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации [memberOf](../api/group-list-memberof.md) (возвращаются только группы, непосредственным членом которых является данная группа).</span><span class="sxs-lookup"><span data-stu-id="d7644-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="d7644-p103">Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос — 2046. Обратите внимание, что компонент "Группы Microsoft 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Microsoft 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="d7644-p103">This function supports Microsoft 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7644-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7644-112">Permissions</span></span>

<span data-ttu-id="d7644-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7644-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7644-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7644-115">Permission type</span></span>                        | <span data-ttu-id="d7644-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7644-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d7644-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7644-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7644-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7644-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d7644-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7644-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7644-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7644-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="d7644-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7644-121">Application</span></span>                            | <span data-ttu-id="d7644-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7644-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="d7644-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7644-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d7644-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7644-124">Request headers</span></span>

| <span data-ttu-id="d7644-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d7644-125">Name</span></span>          | <span data-ttu-id="d7644-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d7644-126">Type</span></span>   | <span data-ttu-id="d7644-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d7644-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d7644-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7644-128">Authorization</span></span> | <span data-ttu-id="d7644-129">string</span><span class="sxs-lookup"><span data-stu-id="d7644-129">string</span></span> | <span data-ttu-id="d7644-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7644-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7644-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7644-132">Request body</span></span>

<span data-ttu-id="d7644-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d7644-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7644-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="d7644-134">Parameter</span></span>           | <span data-ttu-id="d7644-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d7644-135">Type</span></span>    | <span data-ttu-id="d7644-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d7644-136">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="d7644-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d7644-137">securityEnabledOnly</span></span> | <span data-ttu-id="d7644-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="d7644-138">Boolean</span></span> | <span data-ttu-id="d7644-p106">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d7644-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="d7644-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7644-141">Response</span></span>

<span data-ttu-id="d7644-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="d7644-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="d7644-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d7644-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d7644-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7644-144">Request</span></span>

<span data-ttu-id="d7644-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7644-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7644-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7644-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="d7644-147">C#</span><span class="sxs-lookup"><span data-stu-id="d7644-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7644-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7644-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7644-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7644-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7644-150">Java</span><span class="sxs-lookup"><span data-stu-id="d7644-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7644-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7644-151">Response</span></span>

<span data-ttu-id="d7644-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7644-152">The following is an example of the response.</span></span>

> <span data-ttu-id="d7644-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7644-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


