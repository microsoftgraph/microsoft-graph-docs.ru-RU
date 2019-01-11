---
title: assignLicense
description: Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака. К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя. Также можно включить и отключить определенные планы, связанных с подпиской. Для получения дополнительных сведений о подписках и лицензий, см в этой статье Technet.
localization_priority: Normal
ms.openlocfilehash: 71287b47a0a42ce4f89635fe6a1769c78874ae36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876204"
---
# <a name="assignlicense"></a><span data-ttu-id="63266-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="63266-106">assignLicense</span></span>

> <span data-ttu-id="63266-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63266-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63266-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63266-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63266-109">Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака.</span><span class="sxs-lookup"><span data-stu-id="63266-109">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="63266-110">К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="63266-110">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="63266-111">Также можно включить и отключить определенные планы, связанных с подпиской.</span><span class="sxs-lookup"><span data-stu-id="63266-111">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="63266-112">Для получения дополнительных сведений о подписках и лицензий, см в этой [статье Technet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="63266-112">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="63266-113">Чтобы получить подписок, доступных в каталоге, выполните [получить запрос subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="63266-113">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="63266-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63266-114">Permissions</span></span>
<span data-ttu-id="63266-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63266-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63266-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63266-117">Permission type</span></span>      | <span data-ttu-id="63266-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63266-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63266-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63266-119">Delegated (work or school account)</span></span> | <span data-ttu-id="63266-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63266-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="63266-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63266-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63266-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63266-122">Not supported.</span></span>    |
|<span data-ttu-id="63266-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63266-123">Application</span></span> | <span data-ttu-id="63266-124">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63266-124">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63266-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63266-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="63266-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63266-126">Request headers</span></span>
| <span data-ttu-id="63266-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63266-127">Header</span></span>       | <span data-ttu-id="63266-128">Значение</span><span class="sxs-lookup"><span data-stu-id="63266-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63266-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63266-129">Authorization</span></span>  | <span data-ttu-id="63266-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63266-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63266-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63266-132">Content-Type</span></span>  | <span data-ttu-id="63266-133">application/json</span><span class="sxs-lookup"><span data-stu-id="63266-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63266-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63266-134">Request body</span></span>
<span data-ttu-id="63266-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="63266-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63266-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="63266-136">Parameter</span></span>    | <span data-ttu-id="63266-137">Тип</span><span class="sxs-lookup"><span data-stu-id="63266-137">Type</span></span>   |<span data-ttu-id="63266-138">Описание</span><span class="sxs-lookup"><span data-stu-id="63266-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63266-139">addLicenses</span><span class="sxs-lookup"><span data-stu-id="63266-139">addLicenses</span></span>|<span data-ttu-id="63266-140">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="63266-140">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="63266-141">Коллекция объектов [assignedLicense](../resources/assignedlicense.md) , которые задают лицензий для добавления.</span><span class="sxs-lookup"><span data-stu-id="63266-141">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="63266-142">Можно отключить servicePlans, связанный с лицензией путем установки свойства **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="63266-142">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="63266-143">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="63266-143">removeLicenses</span></span>|<span data-ttu-id="63266-144">Guid</span><span class="sxs-lookup"><span data-stu-id="63266-144">Guid</span></span>|<span data-ttu-id="63266-145">Коллекция skuIds, определение лицензий для удаления.</span><span class="sxs-lookup"><span data-stu-id="63266-145">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="63266-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="63266-146">Response</span></span>

<span data-ttu-id="63266-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект обновленный [пользователя](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="63266-147">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63266-148">Пример</span><span class="sxs-lookup"><span data-stu-id="63266-148">Example</span></span>
<span data-ttu-id="63266-149">Добавьте лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="63266-149">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="63266-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="63266-150">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="63266-151">Пример</span><span class="sxs-lookup"><span data-stu-id="63266-151">Example</span></span>
<span data-ttu-id="63266-152">Удалите лицензии у пользователя.</span><span class="sxs-lookup"><span data-stu-id="63266-152">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="63266-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="63266-153">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="63266-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="63266-154">Response</span></span>
<span data-ttu-id="63266-155">В обоих примерах ответа — это объект обновленный пользовательский.</span><span class="sxs-lookup"><span data-stu-id="63266-155">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="63266-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="63266-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="63266-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63266-157">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
