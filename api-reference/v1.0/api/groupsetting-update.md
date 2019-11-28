---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6aa2f8b393f1de1e81174097a9da520a096a33cb
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636801"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="6d210-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="6d210-103">Update a group setting</span></span>

<span data-ttu-id="6d210-104">Обновление свойств для указанных объектов параметров группы.</span><span class="sxs-lookup"><span data-stu-id="6d210-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d210-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d210-105">Permissions</span></span>

<span data-ttu-id="6d210-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6d210-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d210-108">Permission type</span></span>      | <span data-ttu-id="6d210-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d210-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d210-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d210-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d210-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d210-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d210-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d210-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d210-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d210-113">Not supported.</span></span>    |
|<span data-ttu-id="6d210-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d210-114">Application</span></span> | <span data-ttu-id="6d210-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d210-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d210-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d210-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6d210-117">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="6d210-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6d210-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d210-118">Request headers</span></span>
| <span data-ttu-id="6d210-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6d210-119">Name</span></span> | <span data-ttu-id="6d210-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6d210-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="6d210-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d210-121">Authorization</span></span>  | <span data-ttu-id="6d210-122">{Token}.</span><span class="sxs-lookup"><span data-stu-id="6d210-122">{token}.</span></span> <span data-ttu-id="6d210-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6d210-123">Required.</span></span> |
| <span data-ttu-id="6d210-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d210-124">Content-Type</span></span>  | <span data-ttu-id="6d210-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d210-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d210-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d210-126">Request body</span></span>
<span data-ttu-id="6d210-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6d210-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="6d210-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d210-128">Property</span></span> | <span data-ttu-id="6d210-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6d210-129">Type</span></span> | <span data-ttu-id="6d210-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6d210-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="6d210-131">values</span><span class="sxs-lookup"><span data-stu-id="6d210-131">values</span></span> | <span data-ttu-id="6d210-132">Коллекция settingValue</span><span class="sxs-lookup"><span data-stu-id="6d210-132">settingValue collection</span></span> | <span data-ttu-id="6d210-p103">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="6d210-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="6d210-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d210-136">Response</span></span>

<span data-ttu-id="6d210-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d210-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d210-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6d210-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6d210-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d210-139">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d210-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d210-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d210-141">C#</span><span class="sxs-lookup"><span data-stu-id="6d210-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d210-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d210-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d210-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d210-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d210-144">Java</span><span class="sxs-lookup"><span data-stu-id="6d210-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6d210-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d210-145">Response</span></span>

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
