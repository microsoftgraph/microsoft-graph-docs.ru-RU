---
title: assignLicense
description: Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака. К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя. Также можно включить и отключить определенные планы, связанных с подпиской. Для получения дополнительных сведений о подписках и лицензий, см в этой статье Technet.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d15202d24148b2f75bd857500117a4f97b61fe51
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510500"
---
# <a name="assignlicense"></a><span data-ttu-id="473d6-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="473d6-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473d6-107">Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака.</span><span class="sxs-lookup"><span data-stu-id="473d6-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="473d6-108">К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="473d6-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="473d6-109">Также можно включить и отключить определенные планы, связанных с подпиской.</span><span class="sxs-lookup"><span data-stu-id="473d6-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="473d6-110">Для получения дополнительных сведений о подписках и лицензий, см в этой [статье Technet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="473d6-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="473d6-111">Чтобы получить подписок, доступных в каталоге, выполните [получить запрос subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="473d6-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="473d6-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="473d6-112">Permissions</span></span>
<span data-ttu-id="473d6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473d6-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="473d6-115">Permission type</span></span>      | <span data-ttu-id="473d6-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="473d6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="473d6-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="473d6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="473d6-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473d6-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="473d6-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="473d6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473d6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473d6-120">Not supported.</span></span>    |
|<span data-ttu-id="473d6-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="473d6-121">Application</span></span> | <span data-ttu-id="473d6-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473d6-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="473d6-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="473d6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="473d6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="473d6-124">Request headers</span></span>
| <span data-ttu-id="473d6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="473d6-125">Header</span></span>       | <span data-ttu-id="473d6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="473d6-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="473d6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="473d6-127">Authorization</span></span>  | <span data-ttu-id="473d6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="473d6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="473d6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="473d6-130">Content-Type</span></span>  | <span data-ttu-id="473d6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="473d6-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="473d6-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="473d6-132">Request body</span></span>
<span data-ttu-id="473d6-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="473d6-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="473d6-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="473d6-134">Parameter</span></span>    | <span data-ttu-id="473d6-135">Тип</span><span class="sxs-lookup"><span data-stu-id="473d6-135">Type</span></span>   |<span data-ttu-id="473d6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="473d6-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="473d6-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="473d6-137">addLicenses</span></span>|<span data-ttu-id="473d6-138">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="473d6-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="473d6-139">Коллекция объектов [assignedLicense](../resources/assignedlicense.md) , которые задают лицензий для добавления.</span><span class="sxs-lookup"><span data-stu-id="473d6-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="473d6-140">Можно отключить servicePlans, связанный с лицензией путем установки свойства **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="473d6-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="473d6-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="473d6-141">removeLicenses</span></span>|<span data-ttu-id="473d6-142">Guid</span><span class="sxs-lookup"><span data-stu-id="473d6-142">Guid</span></span>|<span data-ttu-id="473d6-143">Коллекция skuIds, определение лицензий для удаления.</span><span class="sxs-lookup"><span data-stu-id="473d6-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="473d6-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="473d6-144">Response</span></span>

<span data-ttu-id="473d6-145">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект обновленный [пользователя](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="473d6-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="473d6-146">Пример</span><span class="sxs-lookup"><span data-stu-id="473d6-146">Example</span></span>
<span data-ttu-id="473d6-147">Добавьте лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="473d6-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="473d6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="473d6-148">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="473d6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="473d6-149">Example</span></span>
<span data-ttu-id="473d6-150">Удалите лицензии у пользователя.</span><span class="sxs-lookup"><span data-stu-id="473d6-150">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="473d6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="473d6-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="473d6-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="473d6-152">Response</span></span>
<span data-ttu-id="473d6-153">В обоих примерах ответа — это объект обновленный пользовательский.</span><span class="sxs-lookup"><span data-stu-id="473d6-153">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="473d6-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="473d6-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="473d6-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="473d6-155">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
