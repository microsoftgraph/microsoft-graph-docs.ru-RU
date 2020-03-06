---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d7690c0db76c7087ff747397eb48e6f014720fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516817"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="8cfa6-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="8cfa6-103">Update a group setting</span></span>

<span data-ttu-id="8cfa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cfa6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cfa6-105">Обновление свойств для указанных объектов параметров группы.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-105">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cfa6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cfa6-106">Permissions</span></span>

<span data-ttu-id="8cfa6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cfa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8cfa6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cfa6-109">Permission type</span></span>      | <span data-ttu-id="8cfa6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cfa6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cfa6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cfa6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8cfa6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cfa6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cfa6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cfa6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cfa6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-114">Not supported.</span></span>    |
|<span data-ttu-id="8cfa6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cfa6-115">Application</span></span> | <span data-ttu-id="8cfa6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cfa6-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cfa6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cfa6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8cfa6-118">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-118">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8cfa6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cfa6-119">Request headers</span></span>
| <span data-ttu-id="8cfa6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8cfa6-120">Name</span></span> | <span data-ttu-id="8cfa6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8cfa6-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="8cfa6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cfa6-122">Authorization</span></span>  | <span data-ttu-id="8cfa6-123">{Token}.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-123">{token}.</span></span> <span data-ttu-id="8cfa6-124">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-124">Required.</span></span> |
| <span data-ttu-id="8cfa6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cfa6-125">Content-Type</span></span>  | <span data-ttu-id="8cfa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cfa6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cfa6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cfa6-127">Request body</span></span>
<span data-ttu-id="8cfa6-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="8cfa6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cfa6-129">Property</span></span> | <span data-ttu-id="8cfa6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8cfa6-130">Type</span></span> | <span data-ttu-id="8cfa6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8cfa6-131">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8cfa6-132">values</span><span class="sxs-lookup"><span data-stu-id="8cfa6-132">values</span></span> | <span data-ttu-id="8cfa6-133">Коллекция settingValue</span><span class="sxs-lookup"><span data-stu-id="8cfa6-133">settingValue collection</span></span> | <span data-ttu-id="8cfa6-p103">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="8cfa6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cfa6-137">Response</span></span>

<span data-ttu-id="8cfa6-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8cfa6-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8cfa6-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8cfa6-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8cfa6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cfa6-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8cfa6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cfa6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
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
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
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
      "value": "True"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="8cfa6-142">C#</span><span class="sxs-lookup"><span data-stu-id="8cfa6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cfa6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cfa6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cfa6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cfa6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cfa6-145">Java</span><span class="sxs-lookup"><span data-stu-id="8cfa6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8cfa6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cfa6-146">Response</span></span>

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
