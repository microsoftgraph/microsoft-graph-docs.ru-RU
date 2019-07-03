---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 13c5b72916ce0ba0b8a6d6516931d99b39ac16f5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442575"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="71437-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="71437-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71437-104">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71437-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71437-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71437-105">Permissions</span></span>

<span data-ttu-id="71437-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="71437-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71437-108">Permission type</span></span>      | <span data-ttu-id="71437-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71437-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71437-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71437-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71437-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71437-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="71437-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71437-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71437-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71437-113">Not supported</span></span> |
|<span data-ttu-id="71437-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71437-114">Application</span></span> | <span data-ttu-id="71437-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71437-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71437-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71437-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="71437-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71437-117">Optional request headers</span></span>
| <span data-ttu-id="71437-118">Имя</span><span class="sxs-lookup"><span data-stu-id="71437-118">Name</span></span> | <span data-ttu-id="71437-119">Описание</span><span class="sxs-lookup"><span data-stu-id="71437-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="71437-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71437-120">Authorization</span></span> | <span data-ttu-id="71437-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71437-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71437-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71437-123">Content-Type</span></span>  | <span data-ttu-id="71437-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71437-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71437-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71437-125">Request body</span></span>

<span data-ttu-id="71437-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="71437-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71437-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="71437-129">Property</span></span> | <span data-ttu-id="71437-130">Тип</span><span class="sxs-lookup"><span data-stu-id="71437-130">Type</span></span> | <span data-ttu-id="71437-131">Описание</span><span class="sxs-lookup"><span data-stu-id="71437-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="71437-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="71437-132">alternateNotificationEmails</span></span>|<span data-ttu-id="71437-133">String</span><span class="sxs-lookup"><span data-stu-id="71437-133">String</span></span>| <span data-ttu-id="71437-134">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="71437-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="71437-135">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="71437-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="71437-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="71437-136">groupLifetimeInDays</span></span>|<span data-ttu-id="71437-137">Int32</span><span class="sxs-lookup"><span data-stu-id="71437-137">Int32</span></span>| <span data-ttu-id="71437-138">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="71437-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="71437-139">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="71437-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="71437-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="71437-140">managedGroupTypes</span></span>|<span data-ttu-id="71437-141">String</span><span class="sxs-lookup"><span data-stu-id="71437-141">String</span></span>| <span data-ttu-id="71437-142">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="71437-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="71437-143">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="71437-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="71437-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="71437-144">Response</span></span>

<span data-ttu-id="71437-145">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71437-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71437-146">Пример</span><span class="sxs-lookup"><span data-stu-id="71437-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71437-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="71437-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71437-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="71437-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="71437-149">C#</span><span class="sxs-lookup"><span data-stu-id="71437-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71437-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="71437-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71437-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="71437-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="71437-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="71437-152">Response</span></span>
<span data-ttu-id="71437-153">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="71437-153">Note: The response object shown here may be truncated for brevity.</span></span> 
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
