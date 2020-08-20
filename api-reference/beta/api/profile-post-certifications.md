---
title: Создание сертификатов
description: Создание нового объекта сертификации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 662b25f18734ed47cd2fb89fce90d04957429830
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820248"
---
# <a name="create-personcertification"></a><span data-ttu-id="0684a-103">Создание personCertification</span><span class="sxs-lookup"><span data-stu-id="0684a-103">Create personCertification</span></span>
<span data-ttu-id="0684a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0684a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0684a-105">Создание объекта [personCertification](../resources/personcertification.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0684a-105">Create a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0684a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0684a-106">Permissions</span></span>

<span data-ttu-id="0684a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0684a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0684a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0684a-109">Permission type</span></span>                        | <span data-ttu-id="0684a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0684a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0684a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0684a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0684a-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0684a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0684a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0684a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0684a-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0684a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0684a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0684a-115">Application</span></span>                            | <span data-ttu-id="0684a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0684a-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="0684a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0684a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a><span data-ttu-id="0684a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0684a-118">Request headers</span></span>
|<span data-ttu-id="0684a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0684a-119">Name</span></span>|<span data-ttu-id="0684a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0684a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0684a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0684a-121">Authorization</span></span>|<span data-ttu-id="0684a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0684a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0684a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0684a-124">Content-Type</span></span>|<span data-ttu-id="0684a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0684a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0684a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0684a-127">Request body</span></span>
<span data-ttu-id="0684a-128">В теле запроса добавьте представление объекта [personCertification в формате](../resources/personcertification.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="0684a-128">In the request body, supply a JSON representation of the [personCertification](../resources/personcertification.md) object.</span></span>

<span data-ttu-id="0684a-129">В таблице ниже приведены свойства, которые можно установить при создании объекта [personCertification](../resources/personcertification.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0684a-129">The following table shows the properties that are possible to set when creating a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="0684a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0684a-130">Property</span></span>|<span data-ttu-id="0684a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0684a-131">Type</span></span>|<span data-ttu-id="0684a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0684a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0684a-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0684a-133">allowedAudiences</span></span>|<span data-ttu-id="0684a-134">String</span><span class="sxs-lookup"><span data-stu-id="0684a-134">String</span></span>|<span data-ttu-id="0684a-135">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="0684a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0684a-136">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0684a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0684a-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0684a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0684a-138">certificationId</span><span class="sxs-lookup"><span data-stu-id="0684a-138">certificationId</span></span>  |<span data-ttu-id="0684a-139">String</span><span class="sxs-lookup"><span data-stu-id="0684a-139">String</span></span>      |<span data-ttu-id="0684a-140">Указывает на идентификатор для сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-140">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="0684a-141">description</span><span class="sxs-lookup"><span data-stu-id="0684a-141">description</span></span>      |<span data-ttu-id="0684a-142">String</span><span class="sxs-lookup"><span data-stu-id="0684a-142">String</span></span>      |<span data-ttu-id="0684a-143">Описание сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-143">Description of the certification.</span></span>                   |
|<span data-ttu-id="0684a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0684a-144">displayName</span></span>      |<span data-ttu-id="0684a-145">String</span><span class="sxs-lookup"><span data-stu-id="0684a-145">String</span></span>      |<span data-ttu-id="0684a-146">Название сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-146">Title of the certification.</span></span>                         |
|<span data-ttu-id="0684a-147">endDate</span><span class="sxs-lookup"><span data-stu-id="0684a-147">endDate</span></span>          |<span data-ttu-id="0684a-148">Date</span><span class="sxs-lookup"><span data-stu-id="0684a-148">Date</span></span>        |<span data-ttu-id="0684a-149">Дата окончания срока действия сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-149">The date that the certification expires.</span></span>            |
|<span data-ttu-id="0684a-150">inference</span><span class="sxs-lookup"><span data-stu-id="0684a-150">inference</span></span>|[<span data-ttu-id="0684a-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0684a-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0684a-152">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="0684a-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0684a-153">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0684a-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0684a-154">issuedDate</span><span class="sxs-lookup"><span data-stu-id="0684a-154">issuedDate</span></span>       |<span data-ttu-id="0684a-155">Дата</span><span class="sxs-lookup"><span data-stu-id="0684a-155">Date</span></span>        |<span data-ttu-id="0684a-156">Дата выпуска сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-156">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="0684a-157">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="0684a-157">issuingAuthority</span></span> |<span data-ttu-id="0684a-158">String</span><span class="sxs-lookup"><span data-stu-id="0684a-158">String</span></span>      |<span data-ttu-id="0684a-159">Центр сертификации, который предоставил сертификат.</span><span class="sxs-lookup"><span data-stu-id="0684a-159">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="0684a-160">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="0684a-160">issuingCompany</span></span>   |<span data-ttu-id="0684a-161">String</span><span class="sxs-lookup"><span data-stu-id="0684a-161">String</span></span>      |<span data-ttu-id="0684a-162">Центр сертификации, который предоставил сертификат.</span><span class="sxs-lookup"><span data-stu-id="0684a-162">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="0684a-163">source</span><span class="sxs-lookup"><span data-stu-id="0684a-163">source</span></span>|[<span data-ttu-id="0684a-164">personDataSource</span><span class="sxs-lookup"><span data-stu-id="0684a-164">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0684a-165">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="0684a-165">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0684a-166">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="0684a-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0684a-167">startDate</span><span class="sxs-lookup"><span data-stu-id="0684a-167">startDate</span></span>        |<span data-ttu-id="0684a-168">Date</span><span class="sxs-lookup"><span data-stu-id="0684a-168">Date</span></span>        |<span data-ttu-id="0684a-169">Дата начала сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-169">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="0684a-170">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="0684a-170">thumbnailUrl</span></span>     |<span data-ttu-id="0684a-171">String</span><span class="sxs-lookup"><span data-stu-id="0684a-171">String</span></span>      |<span data-ttu-id="0684a-172">URL-адрес ссылается на эскиз сертификации.</span><span class="sxs-lookup"><span data-stu-id="0684a-172">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="0684a-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="0684a-173">webUrl</span></span>           |<span data-ttu-id="0684a-174">String</span><span class="sxs-lookup"><span data-stu-id="0684a-174">String</span></span>      |<span data-ttu-id="0684a-175">URL-адрес, ссылающиеся на сертификацию.</span><span class="sxs-lookup"><span data-stu-id="0684a-175">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="0684a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="0684a-176">Response</span></span>

<span data-ttu-id="0684a-177">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект personCertification](../resources/personcertification.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0684a-177">If successful, this method returns a `201 Created` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0684a-178">Примеры</span><span class="sxs-lookup"><span data-stu-id="0684a-178">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="0684a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="0684a-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0684a-180">C#</span><span class="sxs-lookup"><span data-stu-id="0684a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personcertification-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0684a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0684a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personcertification-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0684a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0684a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personcertification-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0684a-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="0684a-183">Response</span></span>
<span data-ttu-id="0684a-184">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0684a-184">**Note:** The response object shown here might be shortened for readability.</span></span>
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
