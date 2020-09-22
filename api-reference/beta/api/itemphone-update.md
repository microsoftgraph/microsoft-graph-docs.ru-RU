---
title: Обновление итемфоне
description: Обновление свойств объекта Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 823dbabbe2936cc7c75af4a480610c7c5d71085c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999359"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="0eeb7-103">Обновление итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="0eeb7-103">Update itemphonenumber</span></span>

<span data-ttu-id="0eeb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eeb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eeb7-105">Обновление свойств объекта [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-105">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0eeb7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eeb7-106">Permissions</span></span>

<span data-ttu-id="0eeb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eeb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0eeb7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eeb7-109">Permission type</span></span>                        | <span data-ttu-id="0eeb7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eeb7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0eeb7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eeb7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0eeb7-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0eeb7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0eeb7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eeb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eeb7-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0eeb7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0eeb7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eeb7-115">Application</span></span>                            | <span data-ttu-id="0eeb7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eeb7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0eeb7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eeb7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/phones/{id}
PATCH /user/{userId}/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0eeb7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eeb7-118">Request headers</span></span>
|<span data-ttu-id="0eeb7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0eeb7-119">Name</span></span>|<span data-ttu-id="0eeb7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0eeb7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0eeb7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eeb7-121">Authorization</span></span>|<span data-ttu-id="0eeb7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0eeb7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0eeb7-124">Content-Type</span></span>|<span data-ttu-id="0eeb7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eeb7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eeb7-127">Request body</span></span>

<span data-ttu-id="0eeb7-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0eeb7-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0eeb7-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="0eeb7-131">В следующей таблице приведены свойства, которые можно задать при обновлении объекта [итемфоне](../resources/itemphone.md) в профиле пользователя.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-131">The following table shows the properties that are possible to set when you update an [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="0eeb7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eeb7-132">Property</span></span>|<span data-ttu-id="0eeb7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0eeb7-133">Type</span></span>|<span data-ttu-id="0eeb7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0eeb7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eeb7-135">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="0eeb7-135">allowedAudiences</span></span>|<span data-ttu-id="0eeb7-136">String</span><span class="sxs-lookup"><span data-stu-id="0eeb7-136">String</span></span>|<span data-ttu-id="0eeb7-137">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0eeb7-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="0eeb7-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0eeb7-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0eeb7-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0eeb7-140">displayName</span></span>|<span data-ttu-id="0eeb7-141">String</span><span class="sxs-lookup"><span data-stu-id="0eeb7-141">String</span></span>|<span data-ttu-id="0eeb7-142">Понятное имя, назначенное пользователю для этого номера телефона.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-142">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="0eeb7-143">выводов</span><span class="sxs-lookup"><span data-stu-id="0eeb7-143">inference</span></span>|[<span data-ttu-id="0eeb7-144">инференцедата</span><span class="sxs-lookup"><span data-stu-id="0eeb7-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0eeb7-145">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0eeb7-146">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="0eeb7-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0eeb7-147">число</span><span class="sxs-lookup"><span data-stu-id="0eeb7-147">number</span></span>|<span data-ttu-id="0eeb7-148">String</span><span class="sxs-lookup"><span data-stu-id="0eeb7-148">String</span></span>|<span data-ttu-id="0eeb7-149">Номер телефона, предоставленный пользователем.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-149">Phone number provided by the user.</span></span>|
|<span data-ttu-id="0eeb7-150">source</span><span class="sxs-lookup"><span data-stu-id="0eeb7-150">source</span></span>|[<span data-ttu-id="0eeb7-151">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="0eeb7-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0eeb7-152">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0eeb7-153">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="0eeb7-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0eeb7-154">type</span><span class="sxs-lookup"><span data-stu-id="0eeb7-154">type</span></span>|<span data-ttu-id="0eeb7-155">фонетипе</span><span class="sxs-lookup"><span data-stu-id="0eeb7-155">phoneType</span></span>|<span data-ttu-id="0eeb7-156">Тип номера телефона в объекте.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-156">The type of phone number within the object.</span></span> <span data-ttu-id="0eeb7-157">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-157">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="0eeb7-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eeb7-158">Response</span></span>

<span data-ttu-id="0eeb7-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-159">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0eeb7-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="0eeb7-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0eeb7-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eeb7-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="0eeb7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eeb7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/phones/{id}
Content-Type: application/json
Content-length: 382

{
  "type": "other"
}
```
# <a name="c"></a>[<span data-ttu-id="0eeb7-163">C#</span><span class="sxs-lookup"><span data-stu-id="0eeb7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0eeb7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0eeb7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0eeb7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0eeb7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0eeb7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eeb7-166">Response</span></span>
<span data-ttu-id="0eeb7-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0eeb7-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
}
-->
``` http
HTTP/1.1 200 OK
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
  "type": "other",
  "number": "+7 499 342 22 13"
}
```


