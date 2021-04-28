---
title: assignLicense
description: Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 57811d4b3a6f22fa021555eec095aebb1854da68
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054324"
---
# <a name="user-assignlicense"></a><span data-ttu-id="a2725-104">user: assignLicense</span><span class="sxs-lookup"><span data-stu-id="a2725-104">user: assignLicense</span></span>

<span data-ttu-id="a2725-p102">Пространство имен: microsoft.graph. Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.</span><span class="sxs-lookup"><span data-stu-id="a2725-p102">Namespace: microsoft.graph Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2725-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2725-107">Permissions</span></span>
<span data-ttu-id="a2725-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2725-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2725-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2725-110">Permission type</span></span>      | <span data-ttu-id="a2725-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2725-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2725-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2725-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2725-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2725-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2725-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2725-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2725-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2725-115">Not supported.</span></span>    |
|<span data-ttu-id="a2725-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2725-116">Application</span></span> | <span data-ttu-id="a2725-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2725-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2725-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2725-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="a2725-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2725-119">Request headers</span></span>
| <span data-ttu-id="a2725-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2725-120">Header</span></span>       | <span data-ttu-id="a2725-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a2725-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2725-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2725-122">Authorization</span></span>  | <span data-ttu-id="a2725-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2725-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a2725-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2725-125">Content-Type</span></span>  | <span data-ttu-id="a2725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2725-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2725-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2725-127">Request body</span></span>
<span data-ttu-id="a2725-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a2725-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2725-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="a2725-129">Parameter</span></span>    | <span data-ttu-id="a2725-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a2725-130">Type</span></span>   |<span data-ttu-id="a2725-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a2725-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2725-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="a2725-132">addLicenses</span></span>|<span data-ttu-id="a2725-133">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a2725-133">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="a2725-p105">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии. Вы можете отключить планы, связанные с лицензией, задав свойство **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="a2725-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="a2725-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="a2725-136">removeLicenses</span></span>|<span data-ttu-id="a2725-137">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="a2725-137">Guid collection</span></span>|<span data-ttu-id="a2725-138">Коллекция идентификаторов GUID, указывающих удаляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="a2725-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="a2725-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2725-139">Response</span></span>

<span data-ttu-id="a2725-140">В случае успеха этот метод возвратит код отклика `200 OK` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2725-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2725-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a2725-141">Example</span></span>
<span data-ttu-id="a2725-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a2725-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2725-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2725-143">Request</span></span>
<span data-ttu-id="a2725-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2725-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2725-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2725-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2725-146">C#</span><span class="sxs-lookup"><span data-stu-id="a2725-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2725-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2725-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2725-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2725-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2725-149">Java</span><span class="sxs-lookup"><span data-stu-id="a2725-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2725-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2725-150">Response</span></span>
<span data-ttu-id="a2725-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2725-151">Here is an example of the response.</span></span> <span data-ttu-id="a2725-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2725-152">Note: The response object shown here might be shortened for readability.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

