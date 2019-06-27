---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9cdbe988e38f6af1941df9eeb2565538295cea28
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273257"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="afd2b-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="afd2b-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="afd2b-104">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afd2b-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afd2b-105">Permissions</span></span>

<span data-ttu-id="afd2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="afd2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afd2b-108">Permission type</span></span>      | <span data-ttu-id="afd2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afd2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afd2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afd2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afd2b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd2b-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="afd2b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afd2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd2b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afd2b-113">Not supported.</span></span>    |
|<span data-ttu-id="afd2b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afd2b-114">Application</span></span> | <span data-ttu-id="afd2b-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd2b-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd2b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afd2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="afd2b-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afd2b-117">Optional request headers</span></span>
| <span data-ttu-id="afd2b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="afd2b-118">Name</span></span> | <span data-ttu-id="afd2b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="afd2b-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="afd2b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afd2b-120">Authorization</span></span> | <span data-ttu-id="afd2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afd2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afd2b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afd2b-123">Content-Type</span></span>  | <span data-ttu-id="afd2b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="afd2b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="afd2b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afd2b-125">Request body</span></span>

<span data-ttu-id="afd2b-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="afd2b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="afd2b-127">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="afd2b-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="afd2b-128">Для наилучших результатов не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="afd2b-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="afd2b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="afd2b-129">Property</span></span> | <span data-ttu-id="afd2b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="afd2b-130">Type</span></span> | <span data-ttu-id="afd2b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="afd2b-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="afd2b-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="afd2b-132">alternateNotificationEmails</span></span>|<span data-ttu-id="afd2b-133">String</span><span class="sxs-lookup"><span data-stu-id="afd2b-133">String</span></span>| <span data-ttu-id="afd2b-134">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="afd2b-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="afd2b-135">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="afd2b-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="afd2b-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="afd2b-136">groupLifetimeInDays</span></span>|<span data-ttu-id="afd2b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="afd2b-137">Int32</span></span>| <span data-ttu-id="afd2b-138">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="afd2b-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="afd2b-139">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="afd2b-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="afd2b-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="afd2b-140">managedGroupTypes</span></span>|<span data-ttu-id="afd2b-141">String</span><span class="sxs-lookup"><span data-stu-id="afd2b-141">String</span></span>| <span data-ttu-id="afd2b-142">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="afd2b-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="afd2b-143">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="afd2b-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="afd2b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="afd2b-144">Response</span></span>

<span data-ttu-id="afd2b-145">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="afd2b-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afd2b-146">Пример</span><span class="sxs-lookup"><span data-stu-id="afd2b-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="afd2b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="afd2b-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="afd2b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="afd2b-148">Response</span></span>
<span data-ttu-id="afd2b-149">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="afd2b-149">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="afd2b-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="afd2b-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="afd2b-151">C#</span><span class="sxs-lookup"><span data-stu-id="afd2b-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afd2b-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="afd2b-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="afd2b-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="afd2b-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
