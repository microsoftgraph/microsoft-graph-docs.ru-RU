---
title: Создание Екстерналграупмембер
description: Создание нового объекта Екстерналграупмембер.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2aa7aacee757b4ae3fd583b285ce2015ebe038aa
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223104"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="2ec34-103">Создание Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="2ec34-103">Create externalGroupMember</span></span>

<span data-ttu-id="2ec34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ec34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ec34-105">Создание нового объекта [екстерналграупмембер](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="2ec34-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ec34-106">Permissions</span></span>

<span data-ttu-id="2ec34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ec34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ec34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ec34-109">Permission type</span></span>                        | <span data-ttu-id="2ec34-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ec34-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ec34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ec34-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ec34-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ec34-112">Not supported</span></span>                               |
| <span data-ttu-id="2ec34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ec34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec34-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ec34-114">Not supported</span></span>                               |
| <span data-ttu-id="2ec34-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ec34-115">Application</span></span>                            | <span data-ttu-id="2ec34-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ec34-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="2ec34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ec34-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="2ec34-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ec34-118">Request headers</span></span>

| <span data-ttu-id="2ec34-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ec34-119">Name</span></span>          | <span data-ttu-id="2ec34-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ec34-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="2ec34-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ec34-121">Authorization</span></span> | <span data-ttu-id="2ec34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ec34-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2ec34-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ec34-124">Content-Type</span></span>  | <span data-ttu-id="2ec34-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ec34-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ec34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ec34-127">Request body</span></span>

<span data-ttu-id="2ec34-128">В тексте запроса добавьте представление объекта [екстерналграупмембер](../resources/externalgroupmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ec34-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="2ec34-129">В следующей таблице приведены свойства, необходимые при создании [екстерналграупмембер](../resources/externalgroupmember.md).</span><span class="sxs-lookup"><span data-stu-id="2ec34-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="2ec34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ec34-130">Property</span></span>       | <span data-ttu-id="2ec34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2ec34-131">Type</span></span>                    | <span data-ttu-id="2ec34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2ec34-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2ec34-133">id</span><span class="sxs-lookup"><span data-stu-id="2ec34-133">id</span></span>             | <span data-ttu-id="2ec34-134">String</span><span class="sxs-lookup"><span data-stu-id="2ec34-134">String</span></span>                  | <span data-ttu-id="2ec34-135">Уникальный `id` элемент.</span><span class="sxs-lookup"><span data-stu-id="2ec34-135">The unique `id` of the member.</span></span> <span data-ttu-id="2ec34-136">Это значение objectId в случае с пользователями или группами Azure Active Directory и Екстерналграупид в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="2ec34-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="2ec34-137">type</span><span class="sxs-lookup"><span data-stu-id="2ec34-137">type</span></span>           | <span data-ttu-id="2ec34-138">екстерналграупмембертипе</span><span class="sxs-lookup"><span data-stu-id="2ec34-138">externalGroupMemberType</span></span> | <span data-ttu-id="2ec34-139">Тип элемента, добавляемого во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="2ec34-139">The type of member added to the external group.</span></span> <span data-ttu-id="2ec34-140">Возможные значения: `user` или `group` , если идентитисаурце, `azureActiveDirectory` и только в том `group` случае, если идентитисаурце `external` .</span><span class="sxs-lookup"><span data-stu-id="2ec34-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="2ec34-141">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="2ec34-141">identitySource</span></span> | <span data-ttu-id="2ec34-142">идентитисаурцетипе</span><span class="sxs-lookup"><span data-stu-id="2ec34-142">identitySourceType</span></span>      | <span data-ttu-id="2ec34-143">Источник удостоверения, к которому принадлежит член.</span><span class="sxs-lookup"><span data-stu-id="2ec34-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="2ec34-144">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="2ec34-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="2ec34-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ec34-145">Response</span></span>

<span data-ttu-id="2ec34-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [екстерналграупмембер](../resources/externalgroupmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ec34-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ec34-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ec34-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="2ec34-148">Пример 1: Добавление пользователя Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="2ec34-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="2ec34-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ec34-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ec34-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ec34-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ec34-151">C#</span><span class="sxs-lookup"><span data-stu-id="2ec34-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ec34-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ec34-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ec34-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ec34-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2ec34-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ec34-154">Response</span></span>

<span data-ttu-id="2ec34-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ec34-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="2ec34-156">Пример 2: Добавление группы Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="2ec34-156">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="2ec34-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ec34-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="2ec34-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ec34-158">Response</span></span>

<span data-ttu-id="2ec34-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ec34-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="2ec34-160">Пример 3: Добавление другой внешней группы в качестве члена</span><span class="sxs-lookup"><span data-stu-id="2ec34-160">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="2ec34-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ec34-161">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="2ec34-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ec34-162">Response</span></span>

<span data-ttu-id="2ec34-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ec34-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
