---
title: Update groupLifecyclePolicy
description: Обновляет свойства объекта groupLifecyclePolicyтип ресурса groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: c428e2d513c359b2b59a7cbb3883458b450ac429
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864913"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="3fc48-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3fc48-103">Update groupLifecyclePolicy</span></span>

> <span data-ttu-id="3fc48-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3fc48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fc48-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fc48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fc48-106">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3fc48-106">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fc48-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fc48-107">Permissions</span></span>

<span data-ttu-id="3fc48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fc48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="3fc48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fc48-110">Permission type</span></span>      | <span data-ttu-id="3fc48-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fc48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fc48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fc48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3fc48-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc48-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3fc48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fc48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fc48-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fc48-115">Not supported</span></span> |
|<span data-ttu-id="3fc48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fc48-116">Application</span></span> | <span data-ttu-id="3fc48-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc48-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fc48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fc48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3fc48-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fc48-119">Optional request headers</span></span>
| <span data-ttu-id="3fc48-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3fc48-120">Name</span></span> | <span data-ttu-id="3fc48-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc48-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="3fc48-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fc48-122">Authorization</span></span> | <span data-ttu-id="3fc48-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fc48-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fc48-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fc48-125">Content-Type</span></span>  | <span data-ttu-id="3fc48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fc48-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fc48-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fc48-127">Request body</span></span>

<span data-ttu-id="3fc48-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3fc48-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3fc48-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fc48-131">Property</span></span> | <span data-ttu-id="3fc48-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3fc48-132">Type</span></span> | <span data-ttu-id="3fc48-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc48-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3fc48-134">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="3fc48-134">alternateNotificationEmails</span></span>|<span data-ttu-id="3fc48-135">String</span><span class="sxs-lookup"><span data-stu-id="3fc48-135">String</span></span>| <span data-ttu-id="3fc48-136">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="3fc48-136">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="3fc48-137">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="3fc48-137">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="3fc48-138">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="3fc48-138">groupLifetimeInDays</span></span>|<span data-ttu-id="3fc48-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3fc48-139">Int32</span></span>| <span data-ttu-id="3fc48-140">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="3fc48-140">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="3fc48-141">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="3fc48-141">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="3fc48-142">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="3fc48-142">managedGroupTypes</span></span>|<span data-ttu-id="3fc48-143">String</span><span class="sxs-lookup"><span data-stu-id="3fc48-143">String</span></span>| <span data-ttu-id="3fc48-144">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="3fc48-144">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="3fc48-145">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="3fc48-145">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="3fc48-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fc48-146">Response</span></span>

<span data-ttu-id="3fc48-147">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fc48-147">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fc48-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3fc48-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3fc48-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fc48-149">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="3fc48-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fc48-150">Response</span></span>
<span data-ttu-id="3fc48-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3fc48-151">Note: The response object shown here may be truncated for brevity.</span></span> 
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
  "tocPath": ""
}-->
