---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29a83493884ffab11b10e8d48f051a45be1f1364
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892617"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="26fc5-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="26fc5-103">Update a group setting</span></span>

<span data-ttu-id="26fc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26fc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26fc5-105">Обновление свойств объекта [groupSetting](../resources/groupsetting.md) для параметров [группы](../resources/group.md) на уровне клиента или определенного параметра группы.</span><span class="sxs-lookup"><span data-stu-id="26fc5-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="26fc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26fc5-106">Permissions</span></span>

<span data-ttu-id="26fc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="26fc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26fc5-109">Permission type</span></span>      | <span data-ttu-id="26fc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26fc5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26fc5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26fc5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26fc5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26fc5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26fc5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26fc5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26fc5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26fc5-114">Not supported.</span></span>    |
|<span data-ttu-id="26fc5-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="26fc5-115">Application</span></span> | <span data-ttu-id="26fc5-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26fc5-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26fc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26fc5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26fc5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26fc5-118">Request headers</span></span>
| <span data-ttu-id="26fc5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26fc5-119">Name</span></span> | <span data-ttu-id="26fc5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26fc5-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="26fc5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26fc5-121">Authorization</span></span>  | <span data-ttu-id="26fc5-122">{Token}.</span><span class="sxs-lookup"><span data-stu-id="26fc5-122">{token}.</span></span> <span data-ttu-id="26fc5-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="26fc5-123">Required.</span></span> |
| <span data-ttu-id="26fc5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26fc5-124">Content-Type</span></span>  | <span data-ttu-id="26fc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26fc5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26fc5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26fc5-126">Request body</span></span>
<span data-ttu-id="26fc5-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="26fc5-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="26fc5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="26fc5-128">Property</span></span> | <span data-ttu-id="26fc5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="26fc5-129">Type</span></span> | <span data-ttu-id="26fc5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="26fc5-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="26fc5-131">values</span><span class="sxs-lookup"><span data-stu-id="26fc5-131">values</span></span> | <span data-ttu-id="26fc5-132">Коллекция [settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="26fc5-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="26fc5-133">Обновленный набор значений.</span><span class="sxs-lookup"><span data-stu-id="26fc5-133">The updated set of values.</span></span> <span data-ttu-id="26fc5-134">Необходимо включить весь набор семейств.</span><span class="sxs-lookup"><span data-stu-id="26fc5-134">You must include the entire collection set.</span></span> <span data-ttu-id="26fc5-135">Невозможно обновить один набор значений.</span><span class="sxs-lookup"><span data-stu-id="26fc5-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="26fc5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="26fc5-136">Response</span></span>

<span data-ttu-id="26fc5-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26fc5-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26fc5-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="26fc5-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="26fc5-139">Пример 1: Обновление параметра группы на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="26fc5-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="26fc5-140">В этом примере `{id}` — это идентификатор объекта groupSetting на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="26fc5-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="26fc5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="26fc5-141">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="26fc5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="26fc5-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="26fc5-143">Пример 2: обновление определенной групповой настройки</span><span class="sxs-lookup"><span data-stu-id="26fc5-143">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="26fc5-144">В этом примере первым `{id}` в запросе является идентификатор группы, а вторым `{id}` — идентификатор объекта groupSetting.</span><span class="sxs-lookup"><span data-stu-id="26fc5-144">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="26fc5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="26fc5-145">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="26fc5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="26fc5-146">Response</span></span>

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
