---
title: Создание Екстерналграупмембер
description: Создание нового объекта Екстерналграупмембер.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c66c21e4b0842df4fb7ececa3378249347f3002d
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193944"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="63303-103">Создание Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="63303-103">Create externalGroupMember</span></span>

<span data-ttu-id="63303-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63303-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63303-105">Создание нового объекта [екстерналграупмембер](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="63303-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63303-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63303-106">Permissions</span></span>

<span data-ttu-id="63303-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63303-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63303-109">Permission type</span></span>                        | <span data-ttu-id="63303-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63303-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63303-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63303-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="63303-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="63303-112">Not supported</span></span>                               |
| <span data-ttu-id="63303-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63303-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63303-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="63303-114">Not supported</span></span>                               |
| <span data-ttu-id="63303-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="63303-115">Application</span></span>                            | <span data-ttu-id="63303-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63303-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="63303-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63303-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="63303-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63303-118">Request headers</span></span>

| <span data-ttu-id="63303-119">Имя</span><span class="sxs-lookup"><span data-stu-id="63303-119">Name</span></span>          | <span data-ttu-id="63303-120">Описание</span><span class="sxs-lookup"><span data-stu-id="63303-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="63303-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63303-121">Authorization</span></span> | <span data-ttu-id="63303-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63303-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="63303-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63303-124">Content-Type</span></span>  | <span data-ttu-id="63303-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63303-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63303-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63303-127">Request body</span></span>

<span data-ttu-id="63303-128">В тексте запроса добавьте представление объекта [екстерналграупмембер](../resources/externalgroupmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63303-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="63303-129">В следующей таблице приведены свойства, необходимые при создании [екстерналграупмембер](../resources/externalgroupmember.md).</span><span class="sxs-lookup"><span data-stu-id="63303-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="63303-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63303-130">Property</span></span>       | <span data-ttu-id="63303-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63303-131">Type</span></span>                    | <span data-ttu-id="63303-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63303-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="63303-133">id</span><span class="sxs-lookup"><span data-stu-id="63303-133">id</span></span>             | <span data-ttu-id="63303-134">String</span><span class="sxs-lookup"><span data-stu-id="63303-134">String</span></span>                  | <span data-ttu-id="63303-135">Уникальный `id` элемент.</span><span class="sxs-lookup"><span data-stu-id="63303-135">The unique `id` of the member.</span></span> <span data-ttu-id="63303-136">Это значение objectId в случае с пользователями или группами Azure Active Directory и Екстерналграупид в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="63303-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="63303-137">type</span><span class="sxs-lookup"><span data-stu-id="63303-137">type</span></span>           | <span data-ttu-id="63303-138">екстерналграупмембертипе</span><span class="sxs-lookup"><span data-stu-id="63303-138">externalGroupMemberType</span></span> | <span data-ttu-id="63303-139">Тип элемента, добавляемого во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="63303-139">The type of member added to the external group.</span></span> <span data-ttu-id="63303-140">Возможные значения: `user` или `group` , если идентитисаурце, `azureActiveDirectory` и только в том `group` случае, если идентитисаурце `external` .</span><span class="sxs-lookup"><span data-stu-id="63303-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="63303-141">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="63303-141">identitySource</span></span> | <span data-ttu-id="63303-142">идентитисаурцетипе</span><span class="sxs-lookup"><span data-stu-id="63303-142">identitySourceType</span></span>      | <span data-ttu-id="63303-143">Источник удостоверения, к которому принадлежит член.</span><span class="sxs-lookup"><span data-stu-id="63303-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="63303-144">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="63303-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="63303-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="63303-145">Response</span></span>

<span data-ttu-id="63303-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [екстерналграупмембер](../resources/externalgroupmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63303-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63303-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="63303-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="63303-148">Пример 1: Добавление пользователя Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="63303-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="63303-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="63303-149">Request</span></span>

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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="63303-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="63303-150">Response</span></span>

<span data-ttu-id="63303-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63303-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="63303-152">Пример 2: Добавление группы Azure Active Directory в качестве участника</span><span class="sxs-lookup"><span data-stu-id="63303-152">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="63303-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="63303-153">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="63303-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="63303-154">Response</span></span>

<span data-ttu-id="63303-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63303-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="63303-156">Пример 3: Добавление другой внешней группы в качестве члена</span><span class="sxs-lookup"><span data-stu-id="63303-156">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="63303-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="63303-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="63303-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="63303-158">Response</span></span>

<span data-ttu-id="63303-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63303-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
