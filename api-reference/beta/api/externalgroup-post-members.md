---
title: Создание externalGroupMember
description: Создание объекта externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7029a0016099dc8ecdbd3ce86983c98b62dc61b1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873180"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="1c165-103">Создание externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="1c165-103">Create externalGroupMember</span></span>

<span data-ttu-id="1c165-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c165-105">Создание объекта [externalGroupMember.](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="1c165-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c165-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c165-106">Permissions</span></span>

<span data-ttu-id="1c165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c165-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c165-109">Permission type</span></span>                        | <span data-ttu-id="1c165-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c165-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c165-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c165-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c165-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c165-112">Not supported</span></span>                               |
| <span data-ttu-id="1c165-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c165-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c165-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c165-114">Not supported</span></span>                               |
| <span data-ttu-id="1c165-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c165-115">Application</span></span>                            | <span data-ttu-id="1c165-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c165-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="1c165-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c165-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="1c165-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c165-118">Request headers</span></span>

| <span data-ttu-id="1c165-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1c165-119">Name</span></span>          | <span data-ttu-id="1c165-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c165-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="1c165-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c165-121">Authorization</span></span> | <span data-ttu-id="1c165-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c165-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1c165-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c165-124">Content-Type</span></span>  | <span data-ttu-id="1c165-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c165-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c165-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c165-127">Request body</span></span>

<span data-ttu-id="1c165-128">В теле запроса укажу представление объекта [externalGroupMember](../resources/externalgroupmember.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1c165-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="1c165-129">В следующей таблице показаны свойства, необходимые при создании [объекта externalGroupMember.](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="1c165-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="1c165-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c165-130">Property</span></span>       | <span data-ttu-id="1c165-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c165-131">Type</span></span>                    | <span data-ttu-id="1c165-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c165-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="1c165-133">id</span><span class="sxs-lookup"><span data-stu-id="1c165-133">id</span></span>             | <span data-ttu-id="1c165-134">String</span><span class="sxs-lookup"><span data-stu-id="1c165-134">String</span></span>                  | <span data-ttu-id="1c165-135">Уникальный `id` член.</span><span class="sxs-lookup"><span data-stu-id="1c165-135">The unique `id` of the member.</span></span> <span data-ttu-id="1c165-136">Это будет objectId в случае пользователей или групп Azure Active Directory и externalGroupId в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="1c165-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="1c165-137">type</span><span class="sxs-lookup"><span data-stu-id="1c165-137">type</span></span>           | <span data-ttu-id="1c165-138">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="1c165-138">externalGroupMemberType</span></span> | <span data-ttu-id="1c165-139">Тип участника, добавленного во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="1c165-139">The type of member added to the external group.</span></span> <span data-ttu-id="1c165-140">Возможные значения: `user` или когда идентификатор `group` identitySource и только `azureActiveDirectory` `group` тогда, когда идентификатор identitySource имеет значение `external` .</span><span class="sxs-lookup"><span data-stu-id="1c165-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="1c165-141">identitySource</span><span class="sxs-lookup"><span data-stu-id="1c165-141">identitySource</span></span> | <span data-ttu-id="1c165-142">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="1c165-142">identitySourceType</span></span>      | <span data-ttu-id="1c165-143">Источник удостоверений, к которой принадлежит участник.</span><span class="sxs-lookup"><span data-stu-id="1c165-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="1c165-144">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="1c165-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="1c165-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c165-145">Response</span></span>

<span data-ttu-id="1c165-146">В случае успеха этот метод возвращает код отклика и объект `201 Created` [externalGroupMember](../resources/externalgroupmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c165-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c165-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c165-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="1c165-148">Пример 1. Добавление пользователя Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="1c165-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="1c165-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c165-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1c165-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c165-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="1c165-151">C#</span><span class="sxs-lookup"><span data-stu-id="1c165-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c165-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c165-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c165-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c165-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c165-154">Java</span><span class="sxs-lookup"><span data-stu-id="1c165-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1c165-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c165-155">Response</span></span>

<span data-ttu-id="1c165-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c165-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="1c165-157">Пример 2. Добавление группы Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="1c165-157">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="1c165-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c165-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="response"></a><span data-ttu-id="1c165-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c165-159">Response</span></span>

<span data-ttu-id="1c165-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c165-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="1c165-161">Пример 3. Добавление другой внешней группы в качестве участника</span><span class="sxs-lookup"><span data-stu-id="1c165-161">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="1c165-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c165-162">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```

### <a name="response"></a><span data-ttu-id="1c165-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c165-163">Response</span></span>

<span data-ttu-id="1c165-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c165-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
