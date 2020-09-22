---
title: 'group: getMemberGroups'
description: Возвращение всех групп, в которых состоит указанная группа.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7a750ef9f2ed34e62b8756c1254da167ccbb0206
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094710"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="67f60-103">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="67f60-103">group: getMemberGroups</span></span>

<span data-ttu-id="67f60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67f60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67f60-p101">Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации [memberOf](../api/group-list-memberof.md) (возвращаются только группы, непосредственным членом которых является данная группа).</span><span class="sxs-lookup"><span data-stu-id="67f60-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="67f60-p102">Эта функция поддерживает Microsoft 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос — 2046. Обратите внимание, что компонент "Группы Microsoft 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Microsoft 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="67f60-p102">This function supports Microsoft 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f60-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67f60-111">Permissions</span></span>

<span data-ttu-id="67f60-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67f60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67f60-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67f60-114">Permission type</span></span>                        | <span data-ttu-id="67f60-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67f60-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="67f60-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67f60-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="67f60-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67f60-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="67f60-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67f60-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f60-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67f60-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="67f60-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="67f60-120">Application</span></span>                            | <span data-ttu-id="67f60-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67f60-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |


## <a name="http-request"></a><span data-ttu-id="67f60-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67f60-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="67f60-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67f60-123">Request headers</span></span>

| <span data-ttu-id="67f60-124">Имя</span><span class="sxs-lookup"><span data-stu-id="67f60-124">Name</span></span>          | <span data-ttu-id="67f60-125">Тип</span><span class="sxs-lookup"><span data-stu-id="67f60-125">Type</span></span>   | <span data-ttu-id="67f60-126">Описание</span><span class="sxs-lookup"><span data-stu-id="67f60-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="67f60-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="67f60-127">Authorization</span></span> | <span data-ttu-id="67f60-128">string</span><span class="sxs-lookup"><span data-stu-id="67f60-128">string</span></span> | <span data-ttu-id="67f60-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67f60-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67f60-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67f60-131">Request body</span></span>

<span data-ttu-id="67f60-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="67f60-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67f60-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="67f60-133">Parameter</span></span>           | <span data-ttu-id="67f60-134">Тип</span><span class="sxs-lookup"><span data-stu-id="67f60-134">Type</span></span>    | <span data-ttu-id="67f60-135">Описание</span><span class="sxs-lookup"><span data-stu-id="67f60-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="67f60-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="67f60-136">securityEnabledOnly</span></span> | <span data-ttu-id="67f60-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="67f60-137">Boolean</span></span> | <span data-ttu-id="67f60-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="67f60-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="67f60-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="67f60-140">Response</span></span>

<span data-ttu-id="67f60-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="67f60-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="67f60-142">Пример</span><span class="sxs-lookup"><span data-stu-id="67f60-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="67f60-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="67f60-143">Request</span></span>

<span data-ttu-id="67f60-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67f60-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67f60-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f60-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67f60-146">C#</span><span class="sxs-lookup"><span data-stu-id="67f60-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67f60-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f60-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67f60-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f60-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67f60-149">Java</span><span class="sxs-lookup"><span data-stu-id="67f60-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67f60-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="67f60-150">Response</span></span>

<span data-ttu-id="67f60-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67f60-151">The following is an example of the response.</span></span>

> <span data-ttu-id="67f60-152">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="67f60-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67f60-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67f60-153">All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

