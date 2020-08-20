---
title: Создание публикаций
description: Создание объекта публикации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 75692418ae2d54650f4ae6c616c727fab5b040e2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819749"
---
# <a name="create-itempublication"></a><span data-ttu-id="0be9e-103">Создание элемента itemPublication</span><span class="sxs-lookup"><span data-stu-id="0be9e-103">Create itemPublication</span></span>
<span data-ttu-id="0be9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0be9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0be9e-105">Создание объекта [itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0be9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0be9e-106">Permissions</span></span>

<span data-ttu-id="0be9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0be9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0be9e-109">Permission type</span></span>                        | <span data-ttu-id="0be9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0be9e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0be9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0be9e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0be9e-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be9e-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0be9e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0be9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be9e-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be9e-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0be9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0be9e-115">Application</span></span>                            | <span data-ttu-id="0be9e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be9e-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="0be9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0be9e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="0be9e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0be9e-118">Request headers</span></span>
|<span data-ttu-id="0be9e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0be9e-119">Name</span></span>|<span data-ttu-id="0be9e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0be9e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0be9e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0be9e-121">Authorization</span></span>|<span data-ttu-id="0be9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0be9e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0be9e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0be9e-124">Content-Type</span></span>|<span data-ttu-id="0be9e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0be9e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be9e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0be9e-127">Request body</span></span>
<span data-ttu-id="0be9e-128">В теле запроса добавьте представление объекта [itemPublication в формате JSON.](../resources/itempublication.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="0be9e-129">В таблице ниже приведены свойства, которые можно установить при создании нового [объекта itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="0be9e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0be9e-130">Property</span></span>|<span data-ttu-id="0be9e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0be9e-131">Type</span></span>|<span data-ttu-id="0be9e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0be9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0be9e-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0be9e-133">allowedAudiences</span></span>|<span data-ttu-id="0be9e-134">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-134">String</span></span>|<span data-ttu-id="0be9e-135">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="0be9e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0be9e-136">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0be9e-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0be9e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0be9e-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="0be9e-138">createdBy</span></span>|[<span data-ttu-id="0be9e-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="0be9e-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0be9e-140">Предоставляет идентификатор пользователя или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="0be9e-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="0be9e-141">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0be9e-142">createdDateTime</span></span>|<span data-ttu-id="0be9e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be9e-143">DateTimeOffset</span></span>|<span data-ttu-id="0be9e-144">Предоставляет dateTimeOffset, когда был создан объект.</span><span class="sxs-lookup"><span data-stu-id="0be9e-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="0be9e-145">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-146">description</span><span class="sxs-lookup"><span data-stu-id="0be9e-146">description</span></span>    |<span data-ttu-id="0be9e-147">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-147">String</span></span>      |<span data-ttu-id="0be9e-148">Описание публикации.</span><span class="sxs-lookup"><span data-stu-id="0be9e-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="0be9e-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0be9e-149">displayName</span></span>    |<span data-ttu-id="0be9e-150">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-150">String</span></span>      |<span data-ttu-id="0be9e-151">Название публикации.</span><span class="sxs-lookup"><span data-stu-id="0be9e-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="0be9e-152">id</span><span class="sxs-lookup"><span data-stu-id="0be9e-152">id</span></span>|<span data-ttu-id="0be9e-153">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-153">String</span></span>|<span data-ttu-id="0be9e-154">Идентификатор, используемый для индивидуального адресации сущности.</span><span class="sxs-lookup"><span data-stu-id="0be9e-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="0be9e-155">Наследуется от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="0be9e-156">inference</span><span class="sxs-lookup"><span data-stu-id="0be9e-156">inference</span></span>|[<span data-ttu-id="0be9e-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0be9e-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0be9e-158">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="0be9e-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0be9e-159">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0be9e-160">lastModifiedBy</span></span>|[<span data-ttu-id="0be9e-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="0be9e-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0be9e-162">Предоставляет идентификатор пользователя или приложения, изменившего сущность.</span><span class="sxs-lookup"><span data-stu-id="0be9e-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="0be9e-163">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0be9e-164">lastModifiedDateTime</span></span>|<span data-ttu-id="0be9e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be9e-165">DateTimeOffset</span></span>|<span data-ttu-id="0be9e-166">Предоставляет dateTimeOffset, когда был создан объект.</span><span class="sxs-lookup"><span data-stu-id="0be9e-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="0be9e-167">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-168">publishedDate</span><span class="sxs-lookup"><span data-stu-id="0be9e-168">publishedDate</span></span>  |<span data-ttu-id="0be9e-169">Дата</span><span class="sxs-lookup"><span data-stu-id="0be9e-169">Date</span></span>        |<span data-ttu-id="0be9e-170">Дата публикации публикации.</span><span class="sxs-lookup"><span data-stu-id="0be9e-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="0be9e-171">publisher</span><span class="sxs-lookup"><span data-stu-id="0be9e-171">publisher</span></span>      |<span data-ttu-id="0be9e-172">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-172">String</span></span>      |<span data-ttu-id="0be9e-173">Публикация или издатель для публикации.</span><span class="sxs-lookup"><span data-stu-id="0be9e-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="0be9e-174">source</span><span class="sxs-lookup"><span data-stu-id="0be9e-174">source</span></span>|[<span data-ttu-id="0be9e-175">personDataSource</span><span class="sxs-lookup"><span data-stu-id="0be9e-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0be9e-176">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="0be9e-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0be9e-177">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0be9e-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0be9e-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="0be9e-178">thumbnailUrl</span></span>   |<span data-ttu-id="0be9e-179">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-179">String</span></span>      |<span data-ttu-id="0be9e-180">URL-адрес ссылается на эскиз публики.</span><span class="sxs-lookup"><span data-stu-id="0be9e-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="0be9e-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="0be9e-181">webUrl</span></span>         |<span data-ttu-id="0be9e-182">String</span><span class="sxs-lookup"><span data-stu-id="0be9e-182">String</span></span>      |<span data-ttu-id="0be9e-183">URL-адрес, ссылающиеся на публикацию.</span><span class="sxs-lookup"><span data-stu-id="0be9e-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="0be9e-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="0be9e-184">Response</span></span>

<span data-ttu-id="0be9e-185">При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект itemPublication](../resources/itempublication.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0be9e-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0be9e-186">Примеры</span><span class="sxs-lookup"><span data-stu-id="0be9e-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="0be9e-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="0be9e-187">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0be9e-188">C#</span><span class="sxs-lookup"><span data-stu-id="0be9e-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0be9e-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0be9e-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0be9e-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0be9e-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0be9e-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="0be9e-191">Response</span></span>
<span data-ttu-id="0be9e-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0be9e-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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
