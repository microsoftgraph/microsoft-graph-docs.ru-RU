---
title: Создание объекта itemPhone
description: С помощью этого API можно создать объект itemPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fcdb1c076d0fff4a3ae5bb6b49fdc77f6acb0aae
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819810"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="e15ea-103">Создание объекта itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e15ea-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="e15ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e15ea-105">С помощью этого API можно [создать новый](../resources/itemphone.md) объект itemPhone в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e15ea-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e15ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e15ea-106">Permissions</span></span>

<span data-ttu-id="e15ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e15ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e15ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e15ea-109">Permission type</span></span>                        | <span data-ttu-id="e15ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e15ea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e15ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e15ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e15ea-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15ea-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e15ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e15ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e15ea-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15ea-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e15ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e15ea-115">Application</span></span>                            | <span data-ttu-id="e15ea-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15ea-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e15ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e15ea-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/phones
POST /users/{userId}/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="e15ea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e15ea-118">Request headers</span></span>
|<span data-ttu-id="e15ea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e15ea-119">Name</span></span>|<span data-ttu-id="e15ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e15ea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e15ea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e15ea-121">Authorization</span></span>|<span data-ttu-id="e15ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e15ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e15ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e15ea-124">Content-Type</span></span>|<span data-ttu-id="e15ea-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e15ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e15ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e15ea-127">Request body</span></span>
<span data-ttu-id="e15ea-128">Представьте в тексте запроса описание объекта [itemPhone в формате JSON.](../resources/itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="e15ea-128">In the request body, supply a JSON representation of the [itemPhone](../resources/itemphone.md) object.</span></span>

<span data-ttu-id="e15ea-129">В приведенной ниже таблице указаны свойства, которые можно установить при создании объекта [itemPhone](../resources/itemphone.md) в профиле пользователей.</span><span class="sxs-lookup"><span data-stu-id="e15ea-129">The following table shows the properties that are possible to set when you create a new [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="e15ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e15ea-130">Property</span></span>|<span data-ttu-id="e15ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e15ea-131">Type</span></span>|<span data-ttu-id="e15ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e15ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e15ea-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e15ea-133">allowedAudiences</span></span>|<span data-ttu-id="e15ea-134">String</span><span class="sxs-lookup"><span data-stu-id="e15ea-134">String</span></span>|<span data-ttu-id="e15ea-135">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="e15ea-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e15ea-136">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="e15ea-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e15ea-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e15ea-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e15ea-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e15ea-138">displayName</span></span>|<span data-ttu-id="e15ea-139">String</span><span class="sxs-lookup"><span data-stu-id="e15ea-139">String</span></span>|<span data-ttu-id="e15ea-140">Понятное имя, назначенное пользователю на этот номер телефона.</span><span class="sxs-lookup"><span data-stu-id="e15ea-140">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="e15ea-141">inference</span><span class="sxs-lookup"><span data-stu-id="e15ea-141">inference</span></span>|[<span data-ttu-id="e15ea-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e15ea-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e15ea-143">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="e15ea-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e15ea-144">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="e15ea-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e15ea-145">число</span><span class="sxs-lookup"><span data-stu-id="e15ea-145">number</span></span>|<span data-ttu-id="e15ea-146">String</span><span class="sxs-lookup"><span data-stu-id="e15ea-146">String</span></span>|<span data-ttu-id="e15ea-147">Номер телефона, указанный пользователем.</span><span class="sxs-lookup"><span data-stu-id="e15ea-147">Phone number provided by the user.</span></span>|
|<span data-ttu-id="e15ea-148">source</span><span class="sxs-lookup"><span data-stu-id="e15ea-148">source</span></span>|[<span data-ttu-id="e15ea-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="e15ea-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e15ea-150">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="e15ea-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e15ea-151">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="e15ea-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e15ea-152">type</span><span class="sxs-lookup"><span data-stu-id="e15ea-152">type</span></span>|<span data-ttu-id="e15ea-153">phoneType</span><span class="sxs-lookup"><span data-stu-id="e15ea-153">phoneType</span></span>|<span data-ttu-id="e15ea-154">Тип номера телефона в объекте.</span><span class="sxs-lookup"><span data-stu-id="e15ea-154">The type of phone number within the object.</span></span> <span data-ttu-id="e15ea-155">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="e15ea-155">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="e15ea-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e15ea-156">Response</span></span>

<span data-ttu-id="e15ea-157">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект itemPhone](../resources/itemphone.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e15ea-157">If successful, this method returns a `201 Created` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e15ea-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="e15ea-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e15ea-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e15ea-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e15ea-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15ea-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-Type: application/json
Content-length: 382

{
  "displayName": "Car Phone",
  "number": "+7 499 342 22 13"
}
```
# <a name="c"></a>[<span data-ttu-id="e15ea-161">C#</span><span class="sxs-lookup"><span data-stu-id="e15ea-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e15ea-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15ea-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e15ea-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15ea-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e15ea-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e15ea-164">Response</span></span>
<span data-ttu-id="e15ea-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e15ea-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "displayName": "Car Phone",
  "type": null,
  "number": "+7 499 342 22 13"
}
```
