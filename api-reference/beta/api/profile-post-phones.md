---
title: Создание Итемфоне
description: Используйте этот API для создания нового Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5b9ad4c2321063234765aa4a5705dcf116e0fd9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974657"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="f358c-103">Создание Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="f358c-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="f358c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f358c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f358c-105">Используйте этот API, чтобы создать новый объект [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f358c-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f358c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f358c-106">Permissions</span></span>

<span data-ttu-id="f358c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f358c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f358c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f358c-109">Permission type</span></span>                        | <span data-ttu-id="f358c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f358c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f358c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f358c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f358c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f358c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f358c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f358c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f358c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f358c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f358c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f358c-115">Application</span></span>                            | <span data-ttu-id="f358c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f358c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f358c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f358c-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/phones
POST /users/{userId}/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="f358c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f358c-118">Request headers</span></span>
|<span data-ttu-id="f358c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f358c-119">Name</span></span>|<span data-ttu-id="f358c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f358c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f358c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f358c-121">Authorization</span></span>|<span data-ttu-id="f358c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f358c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f358c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f358c-124">Content-Type</span></span>|<span data-ttu-id="f358c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f358c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f358c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f358c-127">Request body</span></span>
<span data-ttu-id="f358c-128">В тексте запроса добавьте представление объекта [итемфоне](../resources/itemphone.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f358c-128">In the request body, supply a JSON representation of the [itemPhone](../resources/itemphone.md) object.</span></span>

<span data-ttu-id="f358c-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемфоне](../resources/itemphone.md) в профиле пользователя.</span><span class="sxs-lookup"><span data-stu-id="f358c-129">The following table shows the properties that are possible to set when you create a new [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="f358c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f358c-130">Property</span></span>|<span data-ttu-id="f358c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f358c-131">Type</span></span>|<span data-ttu-id="f358c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f358c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f358c-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="f358c-133">allowedAudiences</span></span>|<span data-ttu-id="f358c-134">String</span><span class="sxs-lookup"><span data-stu-id="f358c-134">String</span></span>|<span data-ttu-id="f358c-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="f358c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f358c-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f358c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f358c-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f358c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f358c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f358c-138">displayName</span></span>|<span data-ttu-id="f358c-139">String</span><span class="sxs-lookup"><span data-stu-id="f358c-139">String</span></span>|<span data-ttu-id="f358c-140">Понятное имя, назначенное пользователю для этого номера телефона.</span><span class="sxs-lookup"><span data-stu-id="f358c-140">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="f358c-141">выводов</span><span class="sxs-lookup"><span data-stu-id="f358c-141">inference</span></span>|[<span data-ttu-id="f358c-142">инференцедата</span><span class="sxs-lookup"><span data-stu-id="f358c-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f358c-143">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="f358c-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f358c-144">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f358c-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f358c-145">число</span><span class="sxs-lookup"><span data-stu-id="f358c-145">number</span></span>|<span data-ttu-id="f358c-146">String</span><span class="sxs-lookup"><span data-stu-id="f358c-146">String</span></span>|<span data-ttu-id="f358c-147">Номер телефона, предоставленный пользователем.</span><span class="sxs-lookup"><span data-stu-id="f358c-147">Phone number provided by the user.</span></span>|
|<span data-ttu-id="f358c-148">source</span><span class="sxs-lookup"><span data-stu-id="f358c-148">source</span></span>|[<span data-ttu-id="f358c-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="f358c-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="f358c-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="f358c-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="f358c-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f358c-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f358c-152">type</span><span class="sxs-lookup"><span data-stu-id="f358c-152">type</span></span>|<span data-ttu-id="f358c-153">фонетипе</span><span class="sxs-lookup"><span data-stu-id="f358c-153">phoneType</span></span>|<span data-ttu-id="f358c-154">Тип номера телефона в объекте.</span><span class="sxs-lookup"><span data-stu-id="f358c-154">The type of phone number within the object.</span></span> <span data-ttu-id="f358c-155">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="f358c-155">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="f358c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f358c-156">Response</span></span>

<span data-ttu-id="f358c-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f358c-157">If successful, this method returns a `201 Created` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f358c-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="f358c-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f358c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f358c-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f358c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="f358c-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f358c-161">C#</span><span class="sxs-lookup"><span data-stu-id="f358c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f358c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f358c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f358c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f358c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f358c-164">Java</span><span class="sxs-lookup"><span data-stu-id="f358c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itemphone-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f358c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="f358c-165">Response</span></span>
<span data-ttu-id="f358c-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f358c-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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


