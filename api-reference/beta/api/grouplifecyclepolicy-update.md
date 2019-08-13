---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 165f72e3741be55c9f1071931ce80e15e84be2eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323003"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="c3c9c-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="c3c9c-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3c9c-104">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c3c9c-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3c9c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c9c-105">Permissions</span></span>

<span data-ttu-id="c3c9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c3c9c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c9c-108">Permission type</span></span>      | <span data-ttu-id="c3c9c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3c9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3c9c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3c9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3c9c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c9c-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3c9c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3c9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3c9c-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c3c9c-113">Not supported</span></span> |
|<span data-ttu-id="c3c9c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3c9c-114">Application</span></span> | <span data-ttu-id="c3c9c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c9c-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3c9c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3c9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c3c9c-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3c9c-117">Optional request headers</span></span>
| <span data-ttu-id="c3c9c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c3c9c-118">Name</span></span> | <span data-ttu-id="c3c9c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c9c-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="c3c9c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3c9c-120">Authorization</span></span> | <span data-ttu-id="c3c9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3c9c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3c9c-123">Content-Type</span></span>  | <span data-ttu-id="c3c9c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c9c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3c9c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3c9c-125">Request body</span></span>

<span data-ttu-id="c3c9c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3c9c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3c9c-129">Property</span></span> | <span data-ttu-id="c3c9c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3c9c-130">Type</span></span> | <span data-ttu-id="c3c9c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c9c-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c3c9c-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="c3c9c-132">alternateNotificationEmails</span></span>|<span data-ttu-id="c3c9c-133">String</span><span class="sxs-lookup"><span data-stu-id="c3c9c-133">String</span></span>| <span data-ttu-id="c3c9c-134">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="c3c9c-135">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="c3c9c-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="c3c9c-136">groupLifetimeInDays</span></span>|<span data-ttu-id="c3c9c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c3c9c-137">Int32</span></span>| <span data-ttu-id="c3c9c-138">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="c3c9c-139">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="c3c9c-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="c3c9c-140">managedGroupTypes</span></span>|<span data-ttu-id="c3c9c-141">String</span><span class="sxs-lookup"><span data-stu-id="c3c9c-141">String</span></span>| <span data-ttu-id="c3c9c-142">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="c3c9c-143">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="c3c9c-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3c9c-144">Response</span></span>

<span data-ttu-id="c3c9c-145">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3c9c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c3c9c-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3c9c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3c9c-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3c9c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3c9c-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3c9c-149">C#</span><span class="sxs-lookup"><span data-stu-id="c3c9c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3c9c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3c9c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3c9c-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c3c9c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3c9c-152">Java</span><span class="sxs-lookup"><span data-stu-id="c3c9c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3c9c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c9c-153">Response</span></span>
<span data-ttu-id="c3c9c-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c3c9c-154">Note: The response object shown here may be truncated for brevity.</span></span> 
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
