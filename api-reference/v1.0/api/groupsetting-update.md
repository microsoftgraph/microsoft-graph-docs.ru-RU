---
title: Обновление параметра группы
description: Обновление свойств для указанных объектов параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4bb0cca83b738caf1579535f2e3cb721f5b0305d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613333"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="3bb65-103">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="3bb65-103">Update a group setting</span></span>

<span data-ttu-id="3bb65-104">Обновление свойств для указанных объектов параметров группы.</span><span class="sxs-lookup"><span data-stu-id="3bb65-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bb65-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bb65-105">Permissions</span></span>

<span data-ttu-id="3bb65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bb65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3bb65-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bb65-108">Permission type</span></span>      | <span data-ttu-id="3bb65-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bb65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bb65-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bb65-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bb65-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bb65-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bb65-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bb65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bb65-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bb65-113">Not supported.</span></span>    |
|<span data-ttu-id="3bb65-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bb65-114">Application</span></span> | <span data-ttu-id="3bb65-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb65-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bb65-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bb65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3bb65-117">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="3bb65-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3bb65-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bb65-118">Optional request headers</span></span>
| <span data-ttu-id="3bb65-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3bb65-119">Name</span></span> | <span data-ttu-id="3bb65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3bb65-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="3bb65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bb65-121">Authorization</span></span>  | <span data-ttu-id="3bb65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bb65-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bb65-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bb65-124">Content-Type</span></span>  | <span data-ttu-id="3bb65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb65-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3bb65-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bb65-126">Request body</span></span>
<span data-ttu-id="3bb65-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3bb65-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="3bb65-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bb65-128">Property</span></span> | <span data-ttu-id="3bb65-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3bb65-129">Type</span></span> | <span data-ttu-id="3bb65-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3bb65-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="3bb65-131">values</span><span class="sxs-lookup"><span data-stu-id="3bb65-131">values</span></span> | <span data-ttu-id="3bb65-132">Коллекция settingValue</span><span class="sxs-lookup"><span data-stu-id="3bb65-132">settingValue collection</span></span> | <span data-ttu-id="3bb65-p103">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="3bb65-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="3bb65-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bb65-136">Response</span></span>

<span data-ttu-id="3bb65-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3bb65-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3bb65-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3bb65-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3bb65-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bb65-139">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="3bb65-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bb65-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bb65-141">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="3bb65-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bb65-142">Языках</span><span class="sxs-lookup"><span data-stu-id="3bb65-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bb65-143">Язык</span><span class="sxs-lookup"><span data-stu-id="3bb65-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_groupsetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
