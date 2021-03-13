---
title: Обновление itemPublication
description: Обновление свойств объекта itemPublication.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bf715534a5af58136f91b7567fa675d85c174696
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770383"
---
# <a name="update-itempublication"></a><span data-ttu-id="a8d2d-103">Обновление itemPublication</span><span class="sxs-lookup"><span data-stu-id="a8d2d-103">Update itemPublication</span></span>

<span data-ttu-id="a8d2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8d2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8d2d-105">Обновление свойств объекта [itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="a8d2d-105">Update the properties of an [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8d2d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8d2d-106">Permissions</span></span>

<span data-ttu-id="a8d2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8d2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8d2d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8d2d-109">Permission type</span></span>                        | <span data-ttu-id="a8d2d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8d2d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a8d2d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8d2d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8d2d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d2d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a8d2d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8d2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8d2d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d2d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a8d2d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8d2d-115">Application</span></span>                            | <span data-ttu-id="a8d2d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d2d-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a8d2d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8d2d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/publications/{id}
PATCH /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a8d2d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8d2d-118">Request headers</span></span>
|<span data-ttu-id="a8d2d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a8d2d-119">Name</span></span>|<span data-ttu-id="a8d2d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d2d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8d2d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8d2d-121">Authorization</span></span>|<span data-ttu-id="a8d2d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8d2d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8d2d-124">Content-Type</span></span>|<span data-ttu-id="a8d2d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d2d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8d2d-127">Request body</span></span>

<span data-ttu-id="a8d2d-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a8d2d-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a8d2d-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="a8d2d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8d2d-131">Property</span></span>|<span data-ttu-id="a8d2d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a8d2d-132">Type</span></span>|<span data-ttu-id="a8d2d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d2d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d2d-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a8d2d-134">allowedAudiences</span></span>|<span data-ttu-id="a8d2d-135">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-135">String</span></span>|<span data-ttu-id="a8d2d-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a8d2d-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a8d2d-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a8d2d-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a8d2d-139">description</span><span class="sxs-lookup"><span data-stu-id="a8d2d-139">description</span></span>    |<span data-ttu-id="a8d2d-140">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-140">String</span></span>      |<span data-ttu-id="a8d2d-141">Описание публикации.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-141">Description of the publication.</span></span>                   |
|<span data-ttu-id="a8d2d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a8d2d-142">displayName</span></span>    |<span data-ttu-id="a8d2d-143">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-143">String</span></span>      |<span data-ttu-id="a8d2d-144">Название публикации.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-144">Title of the publication.</span></span>                         |
|<span data-ttu-id="a8d2d-145">вывод</span><span class="sxs-lookup"><span data-stu-id="a8d2d-145">inference</span></span>|[<span data-ttu-id="a8d2d-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a8d2d-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a8d2d-147">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a8d2d-148">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a8d2d-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a8d2d-149">publishedDate</span><span class="sxs-lookup"><span data-stu-id="a8d2d-149">publishedDate</span></span>  |<span data-ttu-id="a8d2d-150">Дата</span><span class="sxs-lookup"><span data-stu-id="a8d2d-150">Date</span></span>        |<span data-ttu-id="a8d2d-151">Дата публикации.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-151">The date that the publication was published.</span></span>      |
|<span data-ttu-id="a8d2d-152">publisher</span><span class="sxs-lookup"><span data-stu-id="a8d2d-152">publisher</span></span>      |<span data-ttu-id="a8d2d-153">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-153">String</span></span>      |<span data-ttu-id="a8d2d-154">Публикация или издатель для публикации.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-154">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="a8d2d-155">source</span><span class="sxs-lookup"><span data-stu-id="a8d2d-155">source</span></span>|[<span data-ttu-id="a8d2d-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a8d2d-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a8d2d-157">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a8d2d-158">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a8d2d-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a8d2d-159">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="a8d2d-159">thumbnailUrl</span></span>   |<span data-ttu-id="a8d2d-160">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-160">String</span></span>      |<span data-ttu-id="a8d2d-161">URL-адрес, ссылающийся на эскиз публикации.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-161">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="a8d2d-162">webUrl</span><span class="sxs-lookup"><span data-stu-id="a8d2d-162">webUrl</span></span>         |<span data-ttu-id="a8d2d-163">String</span><span class="sxs-lookup"><span data-stu-id="a8d2d-163">String</span></span>      |<span data-ttu-id="a8d2d-164">URL-адрес, ссылающийся на публикацию.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-164">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="a8d2d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8d2d-165">Response</span></span>

<span data-ttu-id="a8d2d-166">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект itemPublication](../resources/itemPublication.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-166">If successful, this method returns a `200 OK` response code and an updated [itemPublication](../resources/itemPublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8d2d-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8d2d-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8d2d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8d2d-168">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="a8d2d-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8d2d-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemPublication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/publications/{id}
Content-Type: application/json
Content-length: 497

{
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
}
```
# <a name="c"></a>[<span data-ttu-id="a8d2d-170">C#</span><span class="sxs-lookup"><span data-stu-id="a8d2d-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8d2d-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8d2d-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8d2d-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8d2d-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8d2d-173">Java</span><span class="sxs-lookup"><span data-stu-id="a8d2d-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-itempublication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a8d2d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8d2d-174">Response</span></span>
<span data-ttu-id="a8d2d-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a8d2d-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "source": null,
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


