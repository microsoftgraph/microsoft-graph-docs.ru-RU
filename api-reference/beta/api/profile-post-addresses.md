---
title: Создание адресов
description: Создание объекта addresses.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2dab94f8aefe12a073041ade6a6deedcee07f8ab
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820265"
---
# <a name="create-addresses"></a><span data-ttu-id="befec-103">Создание адресов</span><span class="sxs-lookup"><span data-stu-id="befec-103">Create addresses</span></span>
<span data-ttu-id="befec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="befec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="befec-105">Создание объекта [itemAddress](../resources/itemaddress.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="befec-105">Create a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="befec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="befec-106">Permissions</span></span>

<span data-ttu-id="befec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="befec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="befec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="befec-109">Permission type</span></span>                        | <span data-ttu-id="befec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="befec-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="befec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="befec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="befec-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befec-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="befec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="befec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="befec-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befec-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="befec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="befec-115">Application</span></span>                            | <span data-ttu-id="befec-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befec-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="befec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="befec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/addresses
POST /users/{id | userPrincipalName}/profile/addresses
```

## <a name="request-headers"></a><span data-ttu-id="befec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="befec-118">Request headers</span></span>
|<span data-ttu-id="befec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="befec-119">Name</span></span>|<span data-ttu-id="befec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="befec-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="befec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="befec-121">Authorization</span></span>|<span data-ttu-id="befec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="befec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="befec-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="befec-124">Content-Type</span></span>|<span data-ttu-id="befec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="befec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="befec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="befec-127">Request body</span></span>
<span data-ttu-id="befec-128">В теле запроса добавьте представление объекта [itemAddress в формате JSON.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="befec-128">In the request body, supply a JSON representation of the [itemAddress](../resources/itemaddress.md) object.</span></span>

<span data-ttu-id="befec-129">В приведенной ниже таблице показаны свойства, которые можно установить при создании [нового объекта itemAddress](../resources/itemaddress.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="befec-129">The following table shows the properties that are possible to set when creating a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="befec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="befec-130">Property</span></span>|<span data-ttu-id="befec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="befec-131">Type</span></span>|<span data-ttu-id="befec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="befec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="befec-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="befec-133">allowedAudiences</span></span>|<span data-ttu-id="befec-134">String</span><span class="sxs-lookup"><span data-stu-id="befec-134">String</span></span>|<span data-ttu-id="befec-135">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="befec-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="befec-136">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="befec-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="befec-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="befec-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="befec-138">detail</span><span class="sxs-lookup"><span data-stu-id="befec-138">detail</span></span>|[<span data-ttu-id="befec-139">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="befec-139">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="befec-140">Сведения о самом адресе.</span><span class="sxs-lookup"><span data-stu-id="befec-140">Details about the address itself.</span></span>|
|<span data-ttu-id="befec-141">displayName</span><span class="sxs-lookup"><span data-stu-id="befec-141">displayName</span></span>|<span data-ttu-id="befec-142">String</span><span class="sxs-lookup"><span data-stu-id="befec-142">String</span></span>|<span data-ttu-id="befec-143">Понятное имя, назначенное пользователю на этот адрес.</span><span class="sxs-lookup"><span data-stu-id="befec-143">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="befec-144">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="befec-144">geoCoordinates</span></span>|[<span data-ttu-id="befec-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="befec-145">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="befec-146">Геоокопдии адреса.</span><span class="sxs-lookup"><span data-stu-id="befec-146">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="befec-147">inference</span><span class="sxs-lookup"><span data-stu-id="befec-147">inference</span></span>|[<span data-ttu-id="befec-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="befec-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="befec-149">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="befec-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="befec-150">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="befec-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="befec-151">source</span><span class="sxs-lookup"><span data-stu-id="befec-151">source</span></span>|[<span data-ttu-id="befec-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="befec-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="befec-153">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="befec-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="befec-154">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="befec-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
## <a name="response"></a><span data-ttu-id="befec-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="befec-155">Response</span></span>

<span data-ttu-id="befec-156">При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект itemAddress](../resources/itemaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="befec-156">If successful, this method returns a `201 Created` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="befec-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="befec-157">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="befec-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="befec-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemaddress_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/addresses
Content-Type: application/json
Content-length: 497

{
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="befec-159">C#</span><span class="sxs-lookup"><span data-stu-id="befec-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemaddress-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="befec-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="befec-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemaddress-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="befec-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="befec-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemaddress-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="befec-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="befec-162">Response</span></span>
<span data-ttu-id="befec-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="befec-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
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
  "source": null,
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```
