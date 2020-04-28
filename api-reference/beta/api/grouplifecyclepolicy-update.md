---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 32d26a167f52ab57835a1c37acf6f2054c1ce91e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123946"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="c1915-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="c1915-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="c1915-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1915-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1915-105">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c1915-105">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1915-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1915-106">Permissions</span></span>

<span data-ttu-id="c1915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c1915-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1915-109">Permission type</span></span>      | <span data-ttu-id="c1915-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1915-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1915-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1915-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1915-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1915-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1915-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1915-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1915-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c1915-114">Not supported</span></span> |
|<span data-ttu-id="c1915-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1915-115">Application</span></span> | <span data-ttu-id="c1915-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1915-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1915-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1915-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c1915-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1915-118">Optional request headers</span></span>
| <span data-ttu-id="c1915-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c1915-119">Name</span></span> | <span data-ttu-id="c1915-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c1915-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="c1915-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1915-121">Authorization</span></span> | <span data-ttu-id="c1915-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1915-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1915-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1915-124">Content-Type</span></span>  | <span data-ttu-id="c1915-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1915-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1915-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1915-126">Request body</span></span>

<span data-ttu-id="c1915-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c1915-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1915-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1915-130">Property</span></span> | <span data-ttu-id="c1915-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1915-131">Type</span></span> | <span data-ttu-id="c1915-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1915-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c1915-133">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="c1915-133">alternateNotificationEmails</span></span>|<span data-ttu-id="c1915-134">String</span><span class="sxs-lookup"><span data-stu-id="c1915-134">String</span></span>| <span data-ttu-id="c1915-135">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="c1915-135">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="c1915-136">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="c1915-136">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="c1915-137">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="c1915-137">groupLifetimeInDays</span></span>|<span data-ttu-id="c1915-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c1915-138">Int32</span></span>| <span data-ttu-id="c1915-139">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="c1915-139">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="c1915-140">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="c1915-140">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="c1915-141">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="c1915-141">managedGroupTypes</span></span>|<span data-ttu-id="c1915-142">String</span><span class="sxs-lookup"><span data-stu-id="c1915-142">String</span></span>| <span data-ttu-id="c1915-143">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="c1915-143">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="c1915-144">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="c1915-144">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="c1915-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1915-145">Response</span></span>

<span data-ttu-id="c1915-146">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1915-146">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1915-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c1915-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1915-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1915-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c1915-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1915-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="c1915-150">C#</span><span class="sxs-lookup"><span data-stu-id="c1915-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1915-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1915-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1915-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1915-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1915-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1915-153">Response</span></span>
<span data-ttu-id="c1915-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c1915-154">Note: The response object shown here may be truncated for brevity.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
