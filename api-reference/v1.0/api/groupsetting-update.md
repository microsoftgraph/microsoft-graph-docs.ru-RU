---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f62adf38b0c417871f207f20ab8eb5bcb530af82
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124520"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="37040-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="37040-103">Update a group setting</span></span>

<span data-ttu-id="37040-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37040-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37040-105">Обновление свойств объекта [groupSetting](../resources/groupsetting.md) для параметров [группы](../resources/group.md) на уровне клиента или определенного параметра группы.</span><span class="sxs-lookup"><span data-stu-id="37040-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="37040-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37040-106">Permissions</span></span>

<span data-ttu-id="37040-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37040-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37040-109">Permission type</span></span>      | <span data-ttu-id="37040-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37040-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37040-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37040-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37040-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37040-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37040-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37040-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37040-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37040-114">Not supported.</span></span>    |
|<span data-ttu-id="37040-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37040-115">Application</span></span> | <span data-ttu-id="37040-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37040-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37040-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37040-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="37040-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37040-118">Request headers</span></span>
| <span data-ttu-id="37040-119">Имя</span><span class="sxs-lookup"><span data-stu-id="37040-119">Name</span></span> | <span data-ttu-id="37040-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37040-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="37040-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37040-121">Authorization</span></span>  | <span data-ttu-id="37040-122">{Token}.</span><span class="sxs-lookup"><span data-stu-id="37040-122">{token}.</span></span> <span data-ttu-id="37040-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="37040-123">Required.</span></span> |
| <span data-ttu-id="37040-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37040-124">Content-Type</span></span>  | <span data-ttu-id="37040-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37040-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37040-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37040-126">Request body</span></span>
<span data-ttu-id="37040-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="37040-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="37040-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="37040-128">Property</span></span> | <span data-ttu-id="37040-129">Тип</span><span class="sxs-lookup"><span data-stu-id="37040-129">Type</span></span> | <span data-ttu-id="37040-130">Описание</span><span class="sxs-lookup"><span data-stu-id="37040-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="37040-131">values</span><span class="sxs-lookup"><span data-stu-id="37040-131">values</span></span> | <span data-ttu-id="37040-132">Коллекция [settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="37040-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="37040-133">Обновленный набор значений.</span><span class="sxs-lookup"><span data-stu-id="37040-133">The updated set of values.</span></span> <span data-ttu-id="37040-134">Необходимо включить весь набор семейств.</span><span class="sxs-lookup"><span data-stu-id="37040-134">You must include the entire collection set.</span></span> <span data-ttu-id="37040-135">Невозможно обновить один набор значений.</span><span class="sxs-lookup"><span data-stu-id="37040-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="37040-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="37040-136">Response</span></span>

<span data-ttu-id="37040-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37040-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="37040-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="37040-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="37040-139">Пример 1: Обновление параметра группы на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="37040-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="37040-140">В этом примере `{id}` — это идентификатор объекта groupSetting на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="37040-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="37040-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="37040-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37040-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="37040-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37040-143">C#</span><span class="sxs-lookup"><span data-stu-id="37040-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-setting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37040-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37040-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-setting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37040-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37040-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-setting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37040-146">Java</span><span class="sxs-lookup"><span data-stu-id="37040-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-setting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37040-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="37040-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="37040-148">Пример 2: обновление определенной групповой настройки</span><span class="sxs-lookup"><span data-stu-id="37040-148">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="37040-149">В этом примере первым `{id}` в запросе является идентификатор группы, а вторым `{id}` — идентификатор объекта groupSetting.</span><span class="sxs-lookup"><span data-stu-id="37040-149">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="37040-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="37040-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37040-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="37040-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37040-152">C#</span><span class="sxs-lookup"><span data-stu-id="37040-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37040-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37040-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37040-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37040-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37040-155">Java</span><span class="sxs-lookup"><span data-stu-id="37040-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37040-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="37040-156">Response</span></span>

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
