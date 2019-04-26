---
title: assignLicense
description: Добавить или удалить лицензии для пользователя, чтобы включить или отключить использование облачных услуг Майкрософт. Например, в Организации может быть установлена подписка на Office 365 корпоративный E3 с лицензиями на 100, и этот запрос назначает одну из этих лицензий определенному пользователю. Вы также можете включать и отключать отдельные планы, связанные с подпиской. Чтобы узнать больше о подписках и лицензиях, ознакомьтесь со статьей TechNet.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9946a7ac53a0e0e8b90a31fd4767bcc0549468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548000"
---
# <a name="assignlicense"></a><span data-ttu-id="af230-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="af230-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af230-107">Добавить или удалить лицензии для пользователя, чтобы включить или отключить использование облачных услуг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="af230-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="af230-108">Например, в Организации может быть установлена подписка на Office 365 корпоративный E3 с лицензиями на 100, и этот запрос назначает одну из этих лицензий определенному пользователю.</span><span class="sxs-lookup"><span data-stu-id="af230-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="af230-109">Вы также можете включать и отключать отдельные планы, связанные с подпиской.</span><span class="sxs-lookup"><span data-stu-id="af230-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="af230-110">Чтобы узнать больше о подписках и лицензиях, ознакомьтесь со [статьЕй TechNet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="af230-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="af230-111">Чтобы получить доступ к подпискам в каталоге, выполните [запрос Get субскрибедскус](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="af230-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="af230-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af230-112">Permissions</span></span>
<span data-ttu-id="af230-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af230-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af230-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af230-115">Permission type</span></span>      | <span data-ttu-id="af230-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af230-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af230-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af230-117">Delegated (work or school account)</span></span> | <span data-ttu-id="af230-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af230-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="af230-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af230-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af230-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af230-120">Not supported.</span></span>    |
|<span data-ttu-id="af230-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af230-121">Application</span></span> | <span data-ttu-id="af230-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af230-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af230-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af230-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="af230-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af230-124">Request headers</span></span>
| <span data-ttu-id="af230-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af230-125">Header</span></span>       | <span data-ttu-id="af230-126">Значение</span><span class="sxs-lookup"><span data-stu-id="af230-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af230-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af230-127">Authorization</span></span>  | <span data-ttu-id="af230-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af230-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af230-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af230-130">Content-Type</span></span>  | <span data-ttu-id="af230-131">application/json</span><span class="sxs-lookup"><span data-stu-id="af230-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af230-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af230-132">Request body</span></span>
<span data-ttu-id="af230-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="af230-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af230-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="af230-134">Parameter</span></span>    | <span data-ttu-id="af230-135">Тип</span><span class="sxs-lookup"><span data-stu-id="af230-135">Type</span></span>   |<span data-ttu-id="af230-136">Описание</span><span class="sxs-lookup"><span data-stu-id="af230-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af230-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="af230-137">addLicenses</span></span>|<span data-ttu-id="af230-138">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="af230-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="af230-139">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="af230-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="af230-140">Вы можете отключить Сервицепланс, связанные с лицензией, задав свойство **дисабледпланс** для объекта [коллекция assignedlicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="af230-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="af230-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="af230-141">removeLicenses</span></span>|<span data-ttu-id="af230-142">Guid</span><span class="sxs-lookup"><span data-stu-id="af230-142">Guid</span></span>|<span data-ttu-id="af230-143">Коллекция Скуидс, идентифицирующая лицензии, которые требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="af230-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="af230-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="af230-144">Response</span></span>

<span data-ttu-id="af230-145">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и обновленный объект [User](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af230-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af230-146">Пример</span><span class="sxs-lookup"><span data-stu-id="af230-146">Example</span></span>
<span data-ttu-id="af230-147">Добавьте лицензии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="af230-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="af230-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="af230-148">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="af230-149">Пример</span><span class="sxs-lookup"><span data-stu-id="af230-149">Example</span></span>
<span data-ttu-id="af230-150">Удаление лицензий от пользователя.</span><span class="sxs-lookup"><span data-stu-id="af230-150">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="af230-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="af230-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="af230-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="af230-152">Response</span></span>
<span data-ttu-id="af230-153">В обоих примерах откликом является обновленный объект пользователя.</span><span class="sxs-lookup"><span data-stu-id="af230-153">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="af230-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="af230-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af230-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af230-155">All of the properties will be returned from an actual call.</span></span>
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
