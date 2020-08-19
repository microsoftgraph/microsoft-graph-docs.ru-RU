---
title: Создание сертификатов
description: Создание нового объекта сертификации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9a97a1219a1d98b4fdd456ac24e4ac78a1b5920e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809744"
---
# <a name="create-personcertification"></a><span data-ttu-id="d94c1-103">Создание Персонцертификатион</span><span class="sxs-lookup"><span data-stu-id="d94c1-103">Create personCertification</span></span>
<span data-ttu-id="d94c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d94c1-105">Создание нового объекта [персонцертификатион](../resources/personcertification.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d94c1-105">Create a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d94c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d94c1-106">Permissions</span></span>

<span data-ttu-id="d94c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d94c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d94c1-109">Permission type</span></span>                        | <span data-ttu-id="d94c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d94c1-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d94c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d94c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d94c1-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d94c1-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d94c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d94c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d94c1-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d94c1-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d94c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d94c1-115">Application</span></span>                            | <span data-ttu-id="d94c1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94c1-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="d94c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d94c1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a><span data-ttu-id="d94c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d94c1-118">Request headers</span></span>
|<span data-ttu-id="d94c1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d94c1-119">Name</span></span>|<span data-ttu-id="d94c1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d94c1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d94c1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d94c1-121">Authorization</span></span>|<span data-ttu-id="d94c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94c1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d94c1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d94c1-124">Content-Type</span></span>|<span data-ttu-id="d94c1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94c1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d94c1-127">Request body</span></span>
<span data-ttu-id="d94c1-128">В тексте запроса добавьте представление объекта [персонцертификатион](../resources/personcertification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d94c1-128">In the request body, supply a JSON representation of the [personCertification](../resources/personcertification.md) object.</span></span>

<span data-ttu-id="d94c1-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [персонцертификатион](../resources/personcertification.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d94c1-129">The following table shows the properties that are possible to set when creating a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="d94c1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d94c1-130">Property</span></span>|<span data-ttu-id="d94c1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d94c1-131">Type</span></span>|<span data-ttu-id="d94c1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d94c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d94c1-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="d94c1-133">allowedAudiences</span></span>|<span data-ttu-id="d94c1-134">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-134">String</span></span>|<span data-ttu-id="d94c1-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="d94c1-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d94c1-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d94c1-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d94c1-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d94c1-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d94c1-138">цертификатионид</span><span class="sxs-lookup"><span data-stu-id="d94c1-138">certificationId</span></span>  |<span data-ttu-id="d94c1-139">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-139">String</span></span>      |<span data-ttu-id="d94c1-140">Справочный идентификатор для сертификации.</span><span class="sxs-lookup"><span data-stu-id="d94c1-140">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="d94c1-141">description</span><span class="sxs-lookup"><span data-stu-id="d94c1-141">description</span></span>      |<span data-ttu-id="d94c1-142">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-142">String</span></span>      |<span data-ttu-id="d94c1-143">Описание сертификата.</span><span class="sxs-lookup"><span data-stu-id="d94c1-143">Description of the certification.</span></span>                   |
|<span data-ttu-id="d94c1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d94c1-144">displayName</span></span>      |<span data-ttu-id="d94c1-145">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-145">String</span></span>      |<span data-ttu-id="d94c1-146">Название сертификата.</span><span class="sxs-lookup"><span data-stu-id="d94c1-146">Title of the certification.</span></span>                         |
|<span data-ttu-id="d94c1-147">endDate</span><span class="sxs-lookup"><span data-stu-id="d94c1-147">endDate</span></span>          |<span data-ttu-id="d94c1-148">Date</span><span class="sxs-lookup"><span data-stu-id="d94c1-148">Date</span></span>        |<span data-ttu-id="d94c1-149">Дата истечения срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d94c1-149">The date that the certification expires.</span></span>            |
|<span data-ttu-id="d94c1-150">выводов</span><span class="sxs-lookup"><span data-stu-id="d94c1-150">inference</span></span>|[<span data-ttu-id="d94c1-151">инференцедата</span><span class="sxs-lookup"><span data-stu-id="d94c1-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d94c1-152">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="d94c1-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d94c1-153">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d94c1-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d94c1-154">иссуеддате</span><span class="sxs-lookup"><span data-stu-id="d94c1-154">issuedDate</span></span>       |<span data-ttu-id="d94c1-155">Дата</span><span class="sxs-lookup"><span data-stu-id="d94c1-155">Date</span></span>        |<span data-ttu-id="d94c1-156">Дата выдачи сертификата.</span><span class="sxs-lookup"><span data-stu-id="d94c1-156">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="d94c1-157">иссуингаусорити</span><span class="sxs-lookup"><span data-stu-id="d94c1-157">issuingAuthority</span></span> |<span data-ttu-id="d94c1-158">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-158">String</span></span>      |<span data-ttu-id="d94c1-159">Центр сертификации, который предоставил сертификат.</span><span class="sxs-lookup"><span data-stu-id="d94c1-159">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="d94c1-160">иссуингкомпани</span><span class="sxs-lookup"><span data-stu-id="d94c1-160">issuingCompany</span></span>   |<span data-ttu-id="d94c1-161">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-161">String</span></span>      |<span data-ttu-id="d94c1-162">Центр сертификации, который предоставил сертификат.</span><span class="sxs-lookup"><span data-stu-id="d94c1-162">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="d94c1-163">source</span><span class="sxs-lookup"><span data-stu-id="d94c1-163">source</span></span>|[<span data-ttu-id="d94c1-164">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="d94c1-164">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d94c1-165">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="d94c1-165">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d94c1-166">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d94c1-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d94c1-167">startDate</span><span class="sxs-lookup"><span data-stu-id="d94c1-167">startDate</span></span>        |<span data-ttu-id="d94c1-168">Date</span><span class="sxs-lookup"><span data-stu-id="d94c1-168">Date</span></span>        |<span data-ttu-id="d94c1-169">Дата, когда сертификация стала действительна.</span><span class="sxs-lookup"><span data-stu-id="d94c1-169">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="d94c1-170">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="d94c1-170">thumbnailUrl</span></span>     |<span data-ttu-id="d94c1-171">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-171">String</span></span>      |<span data-ttu-id="d94c1-172">URL-адрес, ссылающийся на эскиз сертификата.</span><span class="sxs-lookup"><span data-stu-id="d94c1-172">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="d94c1-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="d94c1-173">webUrl</span></span>           |<span data-ttu-id="d94c1-174">String</span><span class="sxs-lookup"><span data-stu-id="d94c1-174">String</span></span>      |<span data-ttu-id="d94c1-175">URL-адрес, ссылающийся на сертификат.</span><span class="sxs-lookup"><span data-stu-id="d94c1-175">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="d94c1-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="d94c1-176">Response</span></span>

<span data-ttu-id="d94c1-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [персонцертификатион](../resources/personcertification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d94c1-177">If successful, this method returns a `201 Created` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d94c1-178">Примеры</span><span class="sxs-lookup"><span data-stu-id="d94c1-178">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="d94c1-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="d94c1-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personCertification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/certifications
Content-Type: application/json
Content-length: 497

{
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
# <a name="c"></a>[<span data-ttu-id="d94c1-180">C#</span><span class="sxs-lookup"><span data-stu-id="d94c1-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d94c1-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d94c1-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d94c1-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d94c1-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d94c1-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="d94c1-183">Response</span></span>
<span data-ttu-id="d94c1-184">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d94c1-184">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": null,
  "issuingCompany": null,
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
