---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 603c2b5616a6eab4f2b5db39c859d3749b0ee18d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124646"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="0735d-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0735d-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="0735d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0735d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0735d-105">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0735d-105">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0735d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0735d-106">Permissions</span></span>

<span data-ttu-id="0735d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0735d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="0735d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0735d-109">Permission type</span></span>      | <span data-ttu-id="0735d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0735d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0735d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0735d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0735d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735d-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0735d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0735d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0735d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0735d-114">Not supported.</span></span>    |
|<span data-ttu-id="0735d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0735d-115">Application</span></span> | <span data-ttu-id="0735d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0735d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0735d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0735d-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0735d-118">Optional request headers</span></span>
| <span data-ttu-id="0735d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0735d-119">Name</span></span> | <span data-ttu-id="0735d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0735d-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="0735d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0735d-121">Authorization</span></span> | <span data-ttu-id="0735d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0735d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0735d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0735d-124">Content-Type</span></span>  | <span data-ttu-id="0735d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0735d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0735d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0735d-126">Request body</span></span>

<span data-ttu-id="0735d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0735d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0735d-128">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0735d-128">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="0735d-129">Для наилучших результатов не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0735d-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0735d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0735d-130">Property</span></span> | <span data-ttu-id="0735d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0735d-131">Type</span></span> | <span data-ttu-id="0735d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0735d-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0735d-133">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="0735d-133">alternateNotificationEmails</span></span>|<span data-ttu-id="0735d-134">String</span><span class="sxs-lookup"><span data-stu-id="0735d-134">String</span></span>| <span data-ttu-id="0735d-135">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="0735d-135">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="0735d-136">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="0735d-136">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="0735d-137">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="0735d-137">groupLifetimeInDays</span></span>|<span data-ttu-id="0735d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0735d-138">Int32</span></span>| <span data-ttu-id="0735d-139">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="0735d-139">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="0735d-140">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="0735d-140">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="0735d-141">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="0735d-141">managedGroupTypes</span></span>|<span data-ttu-id="0735d-142">String</span><span class="sxs-lookup"><span data-stu-id="0735d-142">String</span></span>| <span data-ttu-id="0735d-143">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="0735d-143">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="0735d-144">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="0735d-144">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="0735d-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="0735d-145">Response</span></span>

<span data-ttu-id="0735d-146">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0735d-146">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0735d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="0735d-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0735d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0735d-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0735d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="0735d-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0735d-150">C#</span><span class="sxs-lookup"><span data-stu-id="0735d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0735d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0735d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0735d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0735d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0735d-153">Java</span><span class="sxs-lookup"><span data-stu-id="0735d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0735d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0735d-154">Response</span></span>
<span data-ttu-id="0735d-155">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0735d-155">Note: The response object shown here may be truncated for brevity.</span></span> 
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
