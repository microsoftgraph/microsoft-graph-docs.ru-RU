---
title: Обновление personCertification
description: Обновление свойств объекта personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ce03e7499cd79f1616c26ea53444a443e39b6f68
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577355"
---
# <a name="update-personcertification"></a><span data-ttu-id="29142-103">Обновление personCertification</span><span class="sxs-lookup"><span data-stu-id="29142-103">Update personCertification</span></span>
<span data-ttu-id="29142-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29142-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29142-105">Обновление свойств объекта [personCertification](../resources/personcertification.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="29142-105">Update the properties of a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29142-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29142-106">Permissions</span></span>

<span data-ttu-id="29142-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29142-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29142-109">Permission type</span></span>                        | <span data-ttu-id="29142-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29142-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="29142-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29142-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29142-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29142-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="29142-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29142-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29142-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29142-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="29142-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29142-115">Application</span></span>                            | <span data-ttu-id="29142-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29142-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="29142-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29142-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/certifications/{id}
PATCH /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="29142-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29142-118">Request headers</span></span>
|<span data-ttu-id="29142-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29142-119">Name</span></span>|<span data-ttu-id="29142-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29142-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29142-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29142-121">Authorization</span></span>|<span data-ttu-id="29142-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29142-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29142-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29142-124">Content-Type</span></span>|<span data-ttu-id="29142-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29142-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29142-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29142-127">Request body</span></span>

<span data-ttu-id="29142-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="29142-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="29142-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="29142-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="29142-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="29142-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="29142-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="29142-131">Property</span></span>|<span data-ttu-id="29142-132">Тип</span><span class="sxs-lookup"><span data-stu-id="29142-132">Type</span></span>|<span data-ttu-id="29142-133">Описание</span><span class="sxs-lookup"><span data-stu-id="29142-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29142-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="29142-134">allowedAudiences</span></span>|<span data-ttu-id="29142-135">String</span><span class="sxs-lookup"><span data-stu-id="29142-135">String</span></span>|<span data-ttu-id="29142-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="29142-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="29142-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="29142-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="29142-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="29142-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="29142-139">certificationId</span><span class="sxs-lookup"><span data-stu-id="29142-139">certificationId</span></span>  |<span data-ttu-id="29142-140">String</span><span class="sxs-lookup"><span data-stu-id="29142-140">String</span></span>      |<span data-ttu-id="29142-141">Справочный идентификатор для сертификации.</span><span class="sxs-lookup"><span data-stu-id="29142-141">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="29142-142">description</span><span class="sxs-lookup"><span data-stu-id="29142-142">description</span></span>      |<span data-ttu-id="29142-143">String</span><span class="sxs-lookup"><span data-stu-id="29142-143">String</span></span>      |<span data-ttu-id="29142-144">Описание сертификации.</span><span class="sxs-lookup"><span data-stu-id="29142-144">Description of the certification.</span></span>                   |
|<span data-ttu-id="29142-145">displayName</span><span class="sxs-lookup"><span data-stu-id="29142-145">displayName</span></span>      |<span data-ttu-id="29142-146">String</span><span class="sxs-lookup"><span data-stu-id="29142-146">String</span></span>      |<span data-ttu-id="29142-147">Название сертификата.</span><span class="sxs-lookup"><span data-stu-id="29142-147">Title of the certification.</span></span>                         |
|<span data-ttu-id="29142-148">endDate</span><span class="sxs-lookup"><span data-stu-id="29142-148">endDate</span></span>          |<span data-ttu-id="29142-149">Date</span><span class="sxs-lookup"><span data-stu-id="29142-149">Date</span></span>        |<span data-ttu-id="29142-150">Дата истечения срока сертификации.</span><span class="sxs-lookup"><span data-stu-id="29142-150">The date that the certification expires.</span></span>            |
|<span data-ttu-id="29142-151">вывод</span><span class="sxs-lookup"><span data-stu-id="29142-151">inference</span></span>|[<span data-ttu-id="29142-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="29142-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="29142-153">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="29142-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="29142-154">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="29142-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="29142-155">issuedDate</span><span class="sxs-lookup"><span data-stu-id="29142-155">issuedDate</span></span>       |<span data-ttu-id="29142-156">Дата</span><span class="sxs-lookup"><span data-stu-id="29142-156">Date</span></span>        |<span data-ttu-id="29142-157">Дата выдачи сертификата.</span><span class="sxs-lookup"><span data-stu-id="29142-157">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="29142-158">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="29142-158">issuingAuthority</span></span> |<span data-ttu-id="29142-159">String</span><span class="sxs-lookup"><span data-stu-id="29142-159">String</span></span>      |<span data-ttu-id="29142-160">Орган, который предоставил сертификацию.</span><span class="sxs-lookup"><span data-stu-id="29142-160">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="29142-161">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="29142-161">issuingCompany</span></span>   |<span data-ttu-id="29142-162">String</span><span class="sxs-lookup"><span data-stu-id="29142-162">String</span></span>      |<span data-ttu-id="29142-163">Орган, который предоставил сертификацию.</span><span class="sxs-lookup"><span data-stu-id="29142-163">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="29142-164">startDate</span><span class="sxs-lookup"><span data-stu-id="29142-164">startDate</span></span>        |<span data-ttu-id="29142-165">Date</span><span class="sxs-lookup"><span data-stu-id="29142-165">Date</span></span>        |<span data-ttu-id="29142-166">Дата, когда сертификация стала допустимой.</span><span class="sxs-lookup"><span data-stu-id="29142-166">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="29142-167">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="29142-167">thumbnailUrl</span></span>     |<span data-ttu-id="29142-168">String</span><span class="sxs-lookup"><span data-stu-id="29142-168">String</span></span>      |<span data-ttu-id="29142-169">URL-адрес, ссылающийся на эскиз сертификата.</span><span class="sxs-lookup"><span data-stu-id="29142-169">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="29142-170">webUrl</span><span class="sxs-lookup"><span data-stu-id="29142-170">webUrl</span></span>           |<span data-ttu-id="29142-171">String</span><span class="sxs-lookup"><span data-stu-id="29142-171">String</span></span>      |<span data-ttu-id="29142-172">URL-адрес, ссылающийся на сертификацию.</span><span class="sxs-lookup"><span data-stu-id="29142-172">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="29142-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="29142-173">Response</span></span>

<span data-ttu-id="29142-174">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [personCertification](../resources/personcertification.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="29142-174">If successful, this method returns a `200 OK` response code and an updated [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29142-175">Примеры</span><span class="sxs-lookup"><span data-stu-id="29142-175">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29142-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="29142-176">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="29142-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="29142-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personcertification"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/certifications/{id}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence"
}
```
# <a name="c"></a>[<span data-ttu-id="29142-178">C#</span><span class="sxs-lookup"><span data-stu-id="29142-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29142-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29142-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29142-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29142-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="29142-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="29142-181">Response</span></span>
<span data-ttu-id="29142-182">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29142-182">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence",
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```


