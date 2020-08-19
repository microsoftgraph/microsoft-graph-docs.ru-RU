---
title: Создание Итемфоне
description: Используйте этот API для создания нового Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f0d2b947c2045499f91d405ddef4eb79b39430ad
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811597"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="5b031-103">Создание Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="5b031-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="5b031-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b031-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b031-105">Используйте этот API, чтобы создать новый объект [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b031-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b031-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b031-106">Permissions</span></span>

<span data-ttu-id="5b031-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b031-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b031-109">Permission type</span></span>                        | <span data-ttu-id="5b031-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b031-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b031-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b031-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b031-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b031-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5b031-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b031-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b031-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b031-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5b031-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b031-115">Application</span></span>                            | <span data-ttu-id="5b031-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b031-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5b031-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b031-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/phones
POST /users/{userId}/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="5b031-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b031-118">Request headers</span></span>
|<span data-ttu-id="5b031-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5b031-119">Name</span></span>|<span data-ttu-id="5b031-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5b031-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b031-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b031-121">Authorization</span></span>|<span data-ttu-id="5b031-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b031-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b031-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b031-124">Content-Type</span></span>|<span data-ttu-id="5b031-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b031-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b031-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b031-127">Request body</span></span>
<span data-ttu-id="5b031-128">В тексте запроса добавьте представление объекта [итемфоне](../resources/itemphone.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b031-128">In the request body, supply a JSON representation of the [itemPhone](../resources/itemphone.md) object.</span></span>

<span data-ttu-id="5b031-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемфоне](../resources/itemphone.md) в профиле пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b031-129">The following table shows the properties that are possible to set when you create a new [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="5b031-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b031-130">Property</span></span>|<span data-ttu-id="5b031-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b031-131">Type</span></span>|<span data-ttu-id="5b031-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b031-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b031-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="5b031-133">allowedAudiences</span></span>|<span data-ttu-id="5b031-134">String</span><span class="sxs-lookup"><span data-stu-id="5b031-134">String</span></span>|<span data-ttu-id="5b031-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="5b031-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5b031-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b031-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5b031-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5b031-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5b031-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5b031-138">displayName</span></span>|<span data-ttu-id="5b031-139">String</span><span class="sxs-lookup"><span data-stu-id="5b031-139">String</span></span>|<span data-ttu-id="5b031-140">Понятное имя, назначенное пользователю для этого номера телефона.</span><span class="sxs-lookup"><span data-stu-id="5b031-140">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="5b031-141">выводов</span><span class="sxs-lookup"><span data-stu-id="5b031-141">inference</span></span>|[<span data-ttu-id="5b031-142">инференцедата</span><span class="sxs-lookup"><span data-stu-id="5b031-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5b031-143">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="5b031-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5b031-144">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b031-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5b031-145">число</span><span class="sxs-lookup"><span data-stu-id="5b031-145">number</span></span>|<span data-ttu-id="5b031-146">String</span><span class="sxs-lookup"><span data-stu-id="5b031-146">String</span></span>|<span data-ttu-id="5b031-147">Номер телефона, предоставленный пользователем.</span><span class="sxs-lookup"><span data-stu-id="5b031-147">Phone number provided by the user.</span></span>|
|<span data-ttu-id="5b031-148">source</span><span class="sxs-lookup"><span data-stu-id="5b031-148">source</span></span>|[<span data-ttu-id="5b031-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="5b031-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5b031-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="5b031-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5b031-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b031-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5b031-152">type</span><span class="sxs-lookup"><span data-stu-id="5b031-152">type</span></span>|<span data-ttu-id="5b031-153">фонетипе</span><span class="sxs-lookup"><span data-stu-id="5b031-153">phoneType</span></span>|<span data-ttu-id="5b031-154">Тип номера телефона в объекте.</span><span class="sxs-lookup"><span data-stu-id="5b031-154">The type of phone number within the object.</span></span> <span data-ttu-id="5b031-155">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="5b031-155">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="5b031-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b031-156">Response</span></span>

<span data-ttu-id="5b031-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b031-157">If successful, this method returns a `201 Created` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b031-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b031-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b031-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b031-159">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="5b031-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b031-160">Response</span></span>
<span data-ttu-id="5b031-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b031-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
