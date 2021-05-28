---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a2a504aa8c736df33ef35d3bd131b6329fd499c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679759"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="8040d-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="8040d-103">Update a group setting</span></span>

<span data-ttu-id="8040d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8040d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8040d-105">Обнови свойства объекта [groupSetting](../resources/groupsetting.md) для [](../resources/group.md) параметров группы для всех клиентов или определенного группового параметра.</span><span class="sxs-lookup"><span data-stu-id="8040d-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="8040d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8040d-106">Permissions</span></span>

<span data-ttu-id="8040d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8040d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8040d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8040d-109">Permission type</span></span>      | <span data-ttu-id="8040d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8040d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8040d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8040d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8040d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8040d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8040d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8040d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8040d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8040d-114">Not supported.</span></span>    |
|<span data-ttu-id="8040d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8040d-115">Application</span></span> | <span data-ttu-id="8040d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8040d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8040d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8040d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8040d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8040d-118">Request headers</span></span>
| <span data-ttu-id="8040d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8040d-119">Name</span></span> | <span data-ttu-id="8040d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8040d-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="8040d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8040d-121">Authorization</span></span>  | <span data-ttu-id="8040d-122">{token}.</span><span class="sxs-lookup"><span data-stu-id="8040d-122">{token}.</span></span> <span data-ttu-id="8040d-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8040d-123">Required.</span></span> |
| <span data-ttu-id="8040d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8040d-124">Content-Type</span></span>  | <span data-ttu-id="8040d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8040d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8040d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8040d-126">Request body</span></span>
<span data-ttu-id="8040d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8040d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="8040d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8040d-128">Property</span></span> | <span data-ttu-id="8040d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8040d-129">Type</span></span> | <span data-ttu-id="8040d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8040d-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8040d-131">values</span><span class="sxs-lookup"><span data-stu-id="8040d-131">values</span></span> | <span data-ttu-id="8040d-132">[settingValue](../resources/settingvalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="8040d-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="8040d-133">Обновленный набор значений.</span><span class="sxs-lookup"><span data-stu-id="8040d-133">The updated set of values.</span></span> <span data-ttu-id="8040d-134">Необходимо включить весь набор коллекций.</span><span class="sxs-lookup"><span data-stu-id="8040d-134">You must include the entire collection set.</span></span> <span data-ttu-id="8040d-135">Нельзя обновить один набор значений.</span><span class="sxs-lookup"><span data-stu-id="8040d-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="8040d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8040d-136">Response</span></span>

<span data-ttu-id="8040d-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8040d-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8040d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8040d-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="8040d-139">Пример 1. Обновление параметра группы для всех клиентов</span><span class="sxs-lookup"><span data-stu-id="8040d-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="8040d-140">В этом примере — идентификатор объекта groupSetting для всей группы `{id}` клиента.</span><span class="sxs-lookup"><span data-stu-id="8040d-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="8040d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8040d-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8040d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8040d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenant_setting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json

{
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "EnableMIPLabels",
      "value": "false"
    },
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "false"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "false"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "true"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": ""
    },
    {
      "name": "AllowToAddGuests",
      "value": "true"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="8040d-143">C#</span><span class="sxs-lookup"><span data-stu-id="8040d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-setting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8040d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8040d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-setting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8040d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8040d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-setting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8040d-146">Java</span><span class="sxs-lookup"><span data-stu-id="8040d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-setting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8040d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8040d-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="8040d-148">Пример 2. Обновление определенного группового параметра</span><span class="sxs-lookup"><span data-stu-id="8040d-148">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="8040d-149">В этом примере первый в запросе — идентификатор группы, а второй — идентификатор объекта `{id}` `{id}` groupSetting.</span><span class="sxs-lookup"><span data-stu-id="8040d-149">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="8040d-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8040d-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8040d-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8040d-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/settings/{id}
Content-type: application/json

{
  "displayName": "GroupSettings",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
            "name": "AllowToAddGuests",
            "value": "false"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="8040d-152">C#</span><span class="sxs-lookup"><span data-stu-id="8040d-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8040d-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8040d-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8040d-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8040d-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8040d-155">Java</span><span class="sxs-lookup"><span data-stu-id="8040d-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8040d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8040d-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

