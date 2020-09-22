---
title: Создание Персонанниверсари
description: Используйте этот API для создания нового Персонанниверсари.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c227cadba62b80cf94f6c5f2faa849789db40b71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034569"
---
# <a name="create-personanniversary"></a><span data-ttu-id="8f5bb-103">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="8f5bb-103">Create personAnniversary</span></span>

<span data-ttu-id="8f5bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f5bb-105">Используйте этот API, чтобы создать новый объект [персонанниверсари](../resources/personanniversary.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f5bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5bb-106">Permissions</span></span>

<span data-ttu-id="8f5bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f5bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5bb-109">Permission type</span></span>                        | <span data-ttu-id="8f5bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f5bb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f5bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f5bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f5bb-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f5bb-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8f5bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f5bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f5bb-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f5bb-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8f5bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f5bb-115">Application</span></span>                            | <span data-ttu-id="8f5bb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5bb-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8f5bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f5bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="8f5bb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f5bb-118">Request headers</span></span>

| <span data-ttu-id="8f5bb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f5bb-119">Name</span></span>      |<span data-ttu-id="8f5bb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5bb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f5bb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f5bb-121">Authorization</span></span>  | <span data-ttu-id="8f5bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8f5bb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f5bb-124">Content-Type</span></span>   | <span data-ttu-id="8f5bb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f5bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f5bb-127">Request body</span></span>

<span data-ttu-id="8f5bb-128">В тексте запроса добавьте представление объекта [персонанниверсари](../resources/personanniversary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="8f5bb-129">В следующей таблице приведены свойства, которые можно задать в новом объекте \* \* Персонанниверсари \* \* \* в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="8f5bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f5bb-130">Property</span></span>|<span data-ttu-id="8f5bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5bb-131">Type</span></span>|<span data-ttu-id="8f5bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f5bb-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="8f5bb-133">allowedAudiences</span></span>|<span data-ttu-id="8f5bb-134">String</span><span class="sxs-lookup"><span data-stu-id="8f5bb-134">String</span></span>|<span data-ttu-id="8f5bb-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8f5bb-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8f5bb-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8f5bb-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8f5bb-138">date</span><span class="sxs-lookup"><span data-stu-id="8f5bb-138">date</span></span>|<span data-ttu-id="8f5bb-139">Date</span><span class="sxs-lookup"><span data-stu-id="8f5bb-139">Date</span></span>|<span data-ttu-id="8f5bb-140">Содержит дату, связанную с типом юбилея.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="8f5bb-141">выводов</span><span class="sxs-lookup"><span data-stu-id="8f5bb-141">inference</span></span>|[<span data-ttu-id="8f5bb-142">инференцедата</span><span class="sxs-lookup"><span data-stu-id="8f5bb-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8f5bb-143">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8f5bb-144">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8f5bb-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8f5bb-145">source</span><span class="sxs-lookup"><span data-stu-id="8f5bb-145">source</span></span>|[<span data-ttu-id="8f5bb-146">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="8f5bb-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8f5bb-147">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8f5bb-148">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8f5bb-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8f5bb-149">type</span><span class="sxs-lookup"><span data-stu-id="8f5bb-149">type</span></span>|<span data-ttu-id="8f5bb-150">анниверсаритипе</span><span class="sxs-lookup"><span data-stu-id="8f5bb-150">anniversaryType</span></span>|<span data-ttu-id="8f5bb-151">Тип юбилея даты.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="8f5bb-152">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="8f5bb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5bb-153">Response</span></span>

<span data-ttu-id="8f5bb-154">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [персонанниверсари](../resources/personanniversary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f5bb-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f5bb-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f5bb-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5bb-156">Request</span></span>

<span data-ttu-id="8f5bb-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f5bb-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5bb-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "birthday",
  "date": "1980-01-08"
}
```
# <a name="c"></a>[<span data-ttu-id="8f5bb-159">C#</span><span class="sxs-lookup"><span data-stu-id="8f5bb-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5bb-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5bb-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5bb-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5bb-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8f5bb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5bb-162">Response</span></span>

<span data-ttu-id="8f5bb-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-163">The following is an example of the response.</span></span>

> <span data-ttu-id="8f5bb-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f5bb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "type": "birthday",
  "date": "Date"
}
```


