---
title: assignLicense
description: Добавление или удаление лицензий для пользователя, чтобы включить или отключить использование облачных предложений Майкрософт. Например, организация может иметь подписку Microsoft 365 Enterprise E3 со 100 лицензиями, и этот запрос назначает одну из этих лицензий конкретному пользователю. Вы также можете включать и отключать отдельные планы, связанные с подпиской. Дополнительные новости о подписках и лицензиях см. в статье Technet.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ae5e752eed161d78651e5ed9b93e107320f5a815
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720391"
---
# <a name="user-assignlicense"></a><span data-ttu-id="9f676-106">user: assignLicense</span><span class="sxs-lookup"><span data-stu-id="9f676-106">user: assignLicense</span></span>

<span data-ttu-id="9f676-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f676-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f676-108">Добавление или удаление лицензий для пользователя, чтобы включить или отключить использование облачных предложений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9f676-108">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="9f676-109">Например, организация может иметь подписку Microsoft 365 Enterprise E3 со 100 лицензиями, и этот запрос назначает одну из этих лицензий конкретному пользователю.</span><span class="sxs-lookup"><span data-stu-id="9f676-109">For example, an organization can have a Microsoft 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="9f676-110">Вы также можете включать и отключать отдельные планы, связанные с подпиской.</span><span class="sxs-lookup"><span data-stu-id="9f676-110">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="9f676-111">Дополнительные статьи о подписках и лицензиях см. в статье [Technet.](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings)</span><span class="sxs-lookup"><span data-stu-id="9f676-111">To learn more about subscriptions and licenses, see this [Technet article](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings).</span></span>

<span data-ttu-id="9f676-112">Чтобы получить подписки, доступные в каталоге, выполните [запрос GET subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="9f676-112">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9f676-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f676-113">Permissions</span></span>
<span data-ttu-id="9f676-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f676-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f676-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f676-116">Permission type</span></span>      | <span data-ttu-id="9f676-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f676-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f676-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f676-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9f676-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f676-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f676-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f676-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f676-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f676-121">Not supported.</span></span>    |
|<span data-ttu-id="9f676-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f676-122">Application</span></span> | <span data-ttu-id="9f676-123">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f676-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f676-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f676-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="9f676-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f676-125">Request headers</span></span>
| <span data-ttu-id="9f676-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f676-126">Header</span></span>       | <span data-ttu-id="9f676-127">Значение</span><span class="sxs-lookup"><span data-stu-id="9f676-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f676-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f676-128">Authorization</span></span>  | <span data-ttu-id="9f676-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f676-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f676-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f676-131">Content-Type</span></span>  | <span data-ttu-id="9f676-132">application/json</span><span class="sxs-lookup"><span data-stu-id="9f676-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f676-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f676-133">Request body</span></span>
<span data-ttu-id="9f676-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9f676-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f676-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f676-135">Parameter</span></span>    | <span data-ttu-id="9f676-136">Тип</span><span class="sxs-lookup"><span data-stu-id="9f676-136">Type</span></span>   |<span data-ttu-id="9f676-137">Описание</span><span class="sxs-lookup"><span data-stu-id="9f676-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f676-138">addLicenses</span><span class="sxs-lookup"><span data-stu-id="9f676-138">addLicenses</span></span>|<span data-ttu-id="9f676-139">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9f676-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="9f676-140">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="9f676-140">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="9f676-141">Вы можете отключить servicePlans, связанные с лицензией, установив свойство **disabledPlans** на [объекте assignedLicense.](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9f676-141">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="9f676-142">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="9f676-142">removeLicenses</span></span>|<span data-ttu-id="9f676-143">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="9f676-143">Guid collection</span></span>|<span data-ttu-id="9f676-144">Коллекция skuIds, которые идентифицируют лицензии для удаления.</span><span class="sxs-lookup"><span data-stu-id="9f676-144">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="9f676-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f676-145">Response</span></span>

<span data-ttu-id="9f676-146">В случае успеха этот метод возвращает `200 OK` код [](../resources/user.md) отклика и обновленный объект пользователя в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f676-146">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f676-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9f676-147">Example</span></span>
<span data-ttu-id="9f676-148">Добавление лицензий пользователю.</span><span class="sxs-lookup"><span data-stu-id="9f676-148">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="9f676-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f676-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9f676-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f676-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[<span data-ttu-id="9f676-151">C#</span><span class="sxs-lookup"><span data-stu-id="9f676-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f676-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f676-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f676-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f676-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f676-154">Java</span><span class="sxs-lookup"><span data-stu-id="9f676-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="example"></a><span data-ttu-id="9f676-155">Пример</span><span class="sxs-lookup"><span data-stu-id="9f676-155">Example</span></span>
<span data-ttu-id="9f676-156">Удаление лицензий у пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f676-156">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="9f676-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f676-157">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="9f676-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f676-158">Response</span></span>
<span data-ttu-id="9f676-159">В обоих примерах ответ — это обновленный объект пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f676-159">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="9f676-160">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9f676-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9f676-161">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f676-161">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
