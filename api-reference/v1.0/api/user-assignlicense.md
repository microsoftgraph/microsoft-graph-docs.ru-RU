---
title: assignLicense
description: Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96ececfce4800560b1f2ae625d12e67d10f3f325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965777"
---
# <a name="assignlicense"></a><span data-ttu-id="5cb06-104">assignLicense</span><span class="sxs-lookup"><span data-stu-id="5cb06-104">assignLicense</span></span>
<span data-ttu-id="5cb06-p102">Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.</span><span class="sxs-lookup"><span data-stu-id="5cb06-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cb06-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cb06-107">Permissions</span></span>
<span data-ttu-id="5cb06-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cb06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cb06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cb06-110">Permission type</span></span>      | <span data-ttu-id="5cb06-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cb06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cb06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cb06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5cb06-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cb06-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cb06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cb06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cb06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cb06-115">Not supported.</span></span>    |
|<span data-ttu-id="5cb06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cb06-116">Application</span></span> | <span data-ttu-id="5cb06-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cb06-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cb06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cb06-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="5cb06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cb06-119">Request headers</span></span>
| <span data-ttu-id="5cb06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cb06-120">Header</span></span>       | <span data-ttu-id="5cb06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5cb06-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cb06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cb06-122">Authorization</span></span>  | <span data-ttu-id="5cb06-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cb06-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cb06-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cb06-125">Content-Type</span></span>  | <span data-ttu-id="5cb06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cb06-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cb06-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5cb06-127">Request body</span></span>
<span data-ttu-id="5cb06-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5cb06-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5cb06-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="5cb06-129">Parameter</span></span>    | <span data-ttu-id="5cb06-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5cb06-130">Type</span></span>   |<span data-ttu-id="5cb06-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5cb06-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cb06-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="5cb06-132">addLicenses</span></span>|<span data-ttu-id="5cb06-133">AssignedLicense коллекции</span><span class="sxs-lookup"><span data-stu-id="5cb06-133">AssignedLicense collection</span></span>|<span data-ttu-id="5cb06-p105">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии. Вы можете отключить планы, связанные с лицензией, задав свойство **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="5cb06-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="5cb06-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="5cb06-136">removeLicenses</span></span>|<span data-ttu-id="5cb06-137">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="5cb06-137">Guid collection</span></span>|<span data-ttu-id="5cb06-138">Коллекция идентификаторов GUID, указывающих удаляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="5cb06-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="5cb06-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cb06-139">Response</span></span>

<span data-ttu-id="5cb06-140">В случае успеха этот метод возвратит код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5cb06-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cb06-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5cb06-141">Example</span></span>
<span data-ttu-id="5cb06-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5cb06-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5cb06-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cb06-143">Request</span></span>
<span data-ttu-id="5cb06-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cb06-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "guid"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="5cb06-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cb06-145">Response</span></span>
<span data-ttu-id="5cb06-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5cb06-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "skuId": "0118A350-71FC-4EC3-8F0C-6A1CB8867561"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-02T12:13:14Z",
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
