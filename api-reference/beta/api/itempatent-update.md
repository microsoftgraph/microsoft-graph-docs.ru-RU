---
title: Обновление itemPatent
description: Обновление свойств объекта itemPatent.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 442c5360438755f8d48b156b9ca7911380add017
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577429"
---
# <a name="update-itempatent"></a><span data-ttu-id="7f50d-103">Обновление itemPatent</span><span class="sxs-lookup"><span data-stu-id="7f50d-103">Update itemPatent</span></span>

<span data-ttu-id="7f50d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f50d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f50d-105">Обновление свойств объекта [itemPatent.](../resources/itempatent.md)</span><span class="sxs-lookup"><span data-stu-id="7f50d-105">Update the properties of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f50d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f50d-106">Permissions</span></span>

<span data-ttu-id="7f50d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f50d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f50d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f50d-109">Permission type</span></span>                        | <span data-ttu-id="7f50d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f50d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7f50d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f50d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f50d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f50d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7f50d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f50d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f50d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f50d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7f50d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f50d-115">Application</span></span>                            | <span data-ttu-id="7f50d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f50d-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7f50d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f50d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/patents/{id}
PATCH /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7f50d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f50d-118">Request headers</span></span>
|<span data-ttu-id="7f50d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7f50d-119">Name</span></span>|<span data-ttu-id="7f50d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f50d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7f50d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f50d-121">Authorization</span></span>|<span data-ttu-id="7f50d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f50d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7f50d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f50d-124">Content-Type</span></span>|<span data-ttu-id="7f50d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f50d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f50d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f50d-127">Request body</span></span>

<span data-ttu-id="7f50d-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7f50d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7f50d-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7f50d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7f50d-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7f50d-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="7f50d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f50d-131">Property</span></span>|<span data-ttu-id="7f50d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7f50d-132">Type</span></span>|<span data-ttu-id="7f50d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7f50d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f50d-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="7f50d-134">allowedAudiences</span></span>|<span data-ttu-id="7f50d-135">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-135">String</span></span>|<span data-ttu-id="7f50d-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="7f50d-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="7f50d-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="7f50d-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="7f50d-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7f50d-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7f50d-139">description</span><span class="sxs-lookup"><span data-stu-id="7f50d-139">description</span></span>|<span data-ttu-id="7f50d-140">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-140">String</span></span>|<span data-ttu-id="7f50d-141">Descpription патента или подачи.</span><span class="sxs-lookup"><span data-stu-id="7f50d-141">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="7f50d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7f50d-142">displayName</span></span>|<span data-ttu-id="7f50d-143">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-143">String</span></span>|<span data-ttu-id="7f50d-144">Название патента или подачи.</span><span class="sxs-lookup"><span data-stu-id="7f50d-144">Title of the patent or filing.</span></span> |
|<span data-ttu-id="7f50d-145">вывод</span><span class="sxs-lookup"><span data-stu-id="7f50d-145">inference</span></span>|[<span data-ttu-id="7f50d-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="7f50d-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="7f50d-147">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="7f50d-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="7f50d-148">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="7f50d-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="7f50d-149">isPending</span><span class="sxs-lookup"><span data-stu-id="7f50d-149">isPending</span></span>        |<span data-ttu-id="7f50d-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f50d-150">Boolean</span></span>     |<span data-ttu-id="7f50d-151">Указывает, что патент находится в стадии ожидания.</span><span class="sxs-lookup"><span data-stu-id="7f50d-151">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="7f50d-152">issuedDate</span><span class="sxs-lookup"><span data-stu-id="7f50d-152">issuedDate</span></span>       |<span data-ttu-id="7f50d-153">Дата</span><span class="sxs-lookup"><span data-stu-id="7f50d-153">Date</span></span>        |<span data-ttu-id="7f50d-154">Дата предоставления патента.</span><span class="sxs-lookup"><span data-stu-id="7f50d-154">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="7f50d-155">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="7f50d-155">issuingAuthority</span></span> |<span data-ttu-id="7f50d-156">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-156">String</span></span>      |<span data-ttu-id="7f50d-157">Орган, выдав патент.</span><span class="sxs-lookup"><span data-stu-id="7f50d-157">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="7f50d-158">число</span><span class="sxs-lookup"><span data-stu-id="7f50d-158">number</span></span>           |<span data-ttu-id="7f50d-159">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-159">String</span></span>      |<span data-ttu-id="7f50d-160">Номер патента.</span><span class="sxs-lookup"><span data-stu-id="7f50d-160">The patent number.</span></span>                      |
|<span data-ttu-id="7f50d-161">source</span><span class="sxs-lookup"><span data-stu-id="7f50d-161">source</span></span>|[<span data-ttu-id="7f50d-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="7f50d-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="7f50d-163">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="7f50d-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="7f50d-164">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="7f50d-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="7f50d-165">webUrl</span><span class="sxs-lookup"><span data-stu-id="7f50d-165">webUrl</span></span>           |<span data-ttu-id="7f50d-166">String</span><span class="sxs-lookup"><span data-stu-id="7f50d-166">String</span></span>      |<span data-ttu-id="7f50d-167">URL-адрес, ссылающийся на патент или подачу.</span><span class="sxs-lookup"><span data-stu-id="7f50d-167">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="7f50d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f50d-168">Response</span></span>

<span data-ttu-id="7f50d-169">В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный [объект itemPatent](../resources/itempatent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7f50d-169">If successful, this method returns a `200 OK` response code and an updated [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f50d-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="7f50d-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f50d-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f50d-171">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="7f50d-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f50d-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itempatent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/patents/{id}
Content-Type: application/json
Content-length: 497

{
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="7f50d-173">C#</span><span class="sxs-lookup"><span data-stu-id="7f50d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f50d-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f50d-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f50d-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f50d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7f50d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f50d-176">Response</span></span>
<span data-ttu-id="7f50d-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f50d-177">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 200 OK
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


