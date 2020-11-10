---
title: Создание публикаций
description: Создайте новый объект публикации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f01b936250b57307713b8156a415c90ab7ce6c42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976268"
---
# <a name="create-itempublication"></a><span data-ttu-id="d81c9-103">Создание Итемпубликатион</span><span class="sxs-lookup"><span data-stu-id="d81c9-103">Create itemPublication</span></span>
<span data-ttu-id="d81c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d81c9-105">Создание нового объекта [итемпубликатион](../resources/itempublication.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d81c9-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d81c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d81c9-106">Permissions</span></span>

<span data-ttu-id="d81c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d81c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d81c9-109">Permission type</span></span>                        | <span data-ttu-id="d81c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d81c9-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d81c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d81c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d81c9-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d81c9-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d81c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d81c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81c9-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d81c9-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d81c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d81c9-115">Application</span></span>                            | <span data-ttu-id="d81c9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81c9-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="d81c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d81c9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="d81c9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d81c9-118">Request headers</span></span>
|<span data-ttu-id="d81c9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d81c9-119">Name</span></span>|<span data-ttu-id="d81c9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d81c9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d81c9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d81c9-121">Authorization</span></span>|<span data-ttu-id="d81c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d81c9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d81c9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d81c9-124">Content-Type</span></span>|<span data-ttu-id="d81c9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d81c9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d81c9-127">Request body</span></span>
<span data-ttu-id="d81c9-128">В тексте запроса добавьте представление объекта [итемпубликатион](../resources/itempublication.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d81c9-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="d81c9-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемпубликатион](../resources/itempublication.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d81c9-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="d81c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d81c9-130">Property</span></span>|<span data-ttu-id="d81c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d81c9-131">Type</span></span>|<span data-ttu-id="d81c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d81c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81c9-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="d81c9-133">allowedAudiences</span></span>|<span data-ttu-id="d81c9-134">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-134">String</span></span>|<span data-ttu-id="d81c9-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="d81c9-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d81c9-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d81c9-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d81c9-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d81c9-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="d81c9-138">createdBy</span></span>|[<span data-ttu-id="d81c9-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="d81c9-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d81c9-140">Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="d81c9-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="d81c9-141">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d81c9-142">createdDateTime</span></span>|<span data-ttu-id="d81c9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81c9-143">DateTimeOffset</span></span>|<span data-ttu-id="d81c9-144">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="d81c9-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="d81c9-145">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-146">description</span><span class="sxs-lookup"><span data-stu-id="d81c9-146">description</span></span>    |<span data-ttu-id="d81c9-147">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-147">String</span></span>      |<span data-ttu-id="d81c9-148">Описание публикации.</span><span class="sxs-lookup"><span data-stu-id="d81c9-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="d81c9-149">displayName</span><span class="sxs-lookup"><span data-stu-id="d81c9-149">displayName</span></span>    |<span data-ttu-id="d81c9-150">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-150">String</span></span>      |<span data-ttu-id="d81c9-151">Название публикации.</span><span class="sxs-lookup"><span data-stu-id="d81c9-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="d81c9-152">id</span><span class="sxs-lookup"><span data-stu-id="d81c9-152">id</span></span>|<span data-ttu-id="d81c9-153">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-153">String</span></span>|<span data-ttu-id="d81c9-154">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="d81c9-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="d81c9-155">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="d81c9-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="d81c9-156">выводов</span><span class="sxs-lookup"><span data-stu-id="d81c9-156">inference</span></span>|[<span data-ttu-id="d81c9-157">инференцедата</span><span class="sxs-lookup"><span data-stu-id="d81c9-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d81c9-158">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="d81c9-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d81c9-159">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d81c9-160">lastModifiedBy</span></span>|[<span data-ttu-id="d81c9-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="d81c9-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d81c9-162">Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="d81c9-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="d81c9-163">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d81c9-164">lastModifiedDateTime</span></span>|<span data-ttu-id="d81c9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81c9-165">DateTimeOffset</span></span>|<span data-ttu-id="d81c9-166">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="d81c9-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="d81c9-167">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-168">публишеддате</span><span class="sxs-lookup"><span data-stu-id="d81c9-168">publishedDate</span></span>  |<span data-ttu-id="d81c9-169">Дата</span><span class="sxs-lookup"><span data-stu-id="d81c9-169">Date</span></span>        |<span data-ttu-id="d81c9-170">Дата публикации публикации.</span><span class="sxs-lookup"><span data-stu-id="d81c9-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="d81c9-171">publisher</span><span class="sxs-lookup"><span data-stu-id="d81c9-171">publisher</span></span>      |<span data-ttu-id="d81c9-172">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-172">String</span></span>      |<span data-ttu-id="d81c9-173">Публикация или издатель для публикации.</span><span class="sxs-lookup"><span data-stu-id="d81c9-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="d81c9-174">source</span><span class="sxs-lookup"><span data-stu-id="d81c9-174">source</span></span>|[<span data-ttu-id="d81c9-175">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="d81c9-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d81c9-176">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="d81c9-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d81c9-177">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d81c9-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d81c9-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="d81c9-178">thumbnailUrl</span></span>   |<span data-ttu-id="d81c9-179">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-179">String</span></span>      |<span data-ttu-id="d81c9-180">URL-адрес, ссылающийся на эскиз публикации.</span><span class="sxs-lookup"><span data-stu-id="d81c9-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="d81c9-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="d81c9-181">webUrl</span></span>         |<span data-ttu-id="d81c9-182">String</span><span class="sxs-lookup"><span data-stu-id="d81c9-182">String</span></span>      |<span data-ttu-id="d81c9-183">URL-адрес, ссылающийся на публикацию.</span><span class="sxs-lookup"><span data-stu-id="d81c9-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="d81c9-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="d81c9-184">Response</span></span>

<span data-ttu-id="d81c9-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемпубликатион](../resources/itempublication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d81c9-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d81c9-186">Примеры</span><span class="sxs-lookup"><span data-stu-id="d81c9-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="d81c9-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81c9-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemPublication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/publications
Content-Type: application/json
Content-length: 497

{
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="d81c9-188">C#</span><span class="sxs-lookup"><span data-stu-id="d81c9-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81c9-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81c9-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81c9-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81c9-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81c9-191">Java</span><span class="sxs-lookup"><span data-stu-id="d81c9-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itempublication-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d81c9-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="d81c9-192">Response</span></span>
<span data-ttu-id="d81c9-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d81c9-193">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


