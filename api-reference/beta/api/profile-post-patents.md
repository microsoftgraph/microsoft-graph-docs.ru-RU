---
title: Создание патентов
description: Создание нового объекта патентов.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b90cd7f5f3775b7aafc9f19ef9c8039488fabc35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034392"
---
# <a name="create-itempatent"></a><span data-ttu-id="e29c7-103">Создание Итемпатент</span><span class="sxs-lookup"><span data-stu-id="e29c7-103">Create itemPatent</span></span>

<span data-ttu-id="e29c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e29c7-105">Создайте новый объект [итемпатент](../resources/itempatent.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e29c7-105">Create a new [itemPatent](../resources/itempatent.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e29c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e29c7-106">Permissions</span></span>

<span data-ttu-id="e29c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e29c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e29c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e29c7-109">Permission type</span></span>                        | <span data-ttu-id="e29c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e29c7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e29c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e29c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e29c7-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e29c7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e29c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e29c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e29c7-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e29c7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e29c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e29c7-115">Application</span></span>                            | <span data-ttu-id="e29c7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e29c7-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="e29c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e29c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/patents
POST /users/{id | userPrincipalName}/profile/patents
```

## <a name="request-headers"></a><span data-ttu-id="e29c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e29c7-118">Request headers</span></span>
|<span data-ttu-id="e29c7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e29c7-119">Name</span></span>|<span data-ttu-id="e29c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e29c7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e29c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e29c7-121">Authorization</span></span>|<span data-ttu-id="e29c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29c7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e29c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e29c7-124">Content-Type</span></span>|<span data-ttu-id="e29c7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29c7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e29c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e29c7-127">Request body</span></span>
<span data-ttu-id="e29c7-128">В тексте запроса добавьте представление объекта [итемпатент](../resources/itempatent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e29c7-128">In the request body, supply a JSON representation of the [itemPatent](../resources/itempatent.md) object.</span></span>

<span data-ttu-id="e29c7-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемпатент](../resources/itempatent.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e29c7-129">The following table shows the properties that are possible to set when creating a new [itemPatent](../resources/itempatent.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="e29c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e29c7-130">Property</span></span>|<span data-ttu-id="e29c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e29c7-131">Type</span></span>|<span data-ttu-id="e29c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e29c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e29c7-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="e29c7-133">allowedAudiences</span></span>|<span data-ttu-id="e29c7-134">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-134">String</span></span>|<span data-ttu-id="e29c7-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="e29c7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e29c7-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e29c7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e29c7-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e29c7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e29c7-138">description</span><span class="sxs-lookup"><span data-stu-id="e29c7-138">description</span></span>|<span data-ttu-id="e29c7-139">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-139">String</span></span>|<span data-ttu-id="e29c7-140">Дескприптион патента или для хранения.</span><span class="sxs-lookup"><span data-stu-id="e29c7-140">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="e29c7-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e29c7-141">displayName</span></span>|<span data-ttu-id="e29c7-142">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-142">String</span></span>|<span data-ttu-id="e29c7-143">Название патента или его для архивации.</span><span class="sxs-lookup"><span data-stu-id="e29c7-143">Title of the patent or filing.</span></span> |
|<span data-ttu-id="e29c7-144">выводов</span><span class="sxs-lookup"><span data-stu-id="e29c7-144">inference</span></span>|[<span data-ttu-id="e29c7-145">инференцедата</span><span class="sxs-lookup"><span data-stu-id="e29c7-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e29c7-146">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="e29c7-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e29c7-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e29c7-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e29c7-148">Ожидается</span><span class="sxs-lookup"><span data-stu-id="e29c7-148">isPending</span></span>        |<span data-ttu-id="e29c7-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e29c7-149">Boolean</span></span>     |<span data-ttu-id="e29c7-150">Указывает, что патент находится в состоянии ожидания.</span><span class="sxs-lookup"><span data-stu-id="e29c7-150">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="e29c7-151">иссуеддате</span><span class="sxs-lookup"><span data-stu-id="e29c7-151">issuedDate</span></span>       |<span data-ttu-id="e29c7-152">Дата</span><span class="sxs-lookup"><span data-stu-id="e29c7-152">Date</span></span>        |<span data-ttu-id="e29c7-153">Дата предоставления патента.</span><span class="sxs-lookup"><span data-stu-id="e29c7-153">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="e29c7-154">иссуингаусорити</span><span class="sxs-lookup"><span data-stu-id="e29c7-154">issuingAuthority</span></span> |<span data-ttu-id="e29c7-155">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-155">String</span></span>      |<span data-ttu-id="e29c7-156">Центр сертификации, который предоставил патент.</span><span class="sxs-lookup"><span data-stu-id="e29c7-156">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="e29c7-157">число</span><span class="sxs-lookup"><span data-stu-id="e29c7-157">number</span></span>           |<span data-ttu-id="e29c7-158">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-158">String</span></span>      |<span data-ttu-id="e29c7-159">Номер патента.</span><span class="sxs-lookup"><span data-stu-id="e29c7-159">The patent number.</span></span>                      |
|<span data-ttu-id="e29c7-160">source</span><span class="sxs-lookup"><span data-stu-id="e29c7-160">source</span></span>|[<span data-ttu-id="e29c7-161">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="e29c7-161">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e29c7-162">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="e29c7-162">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e29c7-163">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e29c7-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e29c7-164">webUrl</span><span class="sxs-lookup"><span data-stu-id="e29c7-164">webUrl</span></span>           |<span data-ttu-id="e29c7-165">String</span><span class="sxs-lookup"><span data-stu-id="e29c7-165">String</span></span>      |<span data-ttu-id="e29c7-166">URL-адрес, ссылающийся на патент или в систему архивации.</span><span class="sxs-lookup"><span data-stu-id="e29c7-166">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="e29c7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29c7-167">Response</span></span>

<span data-ttu-id="e29c7-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемпатент](../resources/itempatent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e29c7-168">If successful, this method returns a `201 Created` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e29c7-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="e29c7-169">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="e29c7-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="e29c7-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itempatent_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/patents
Content-Type: application/json
Content-length: 497

{
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="e29c7-171">C#</span><span class="sxs-lookup"><span data-stu-id="e29c7-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempatent-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e29c7-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e29c7-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempatent-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e29c7-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e29c7-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempatent-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e29c7-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29c7-174">Response</span></span>
<span data-ttu-id="e29c7-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e29c7-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```


