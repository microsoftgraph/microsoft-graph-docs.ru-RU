---
title: Создание набирателя
description: Создание объекта awards.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b40795f5961bfe47388b01abaf1ce39725a8d113
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819577"
---
# <a name="create-personaward"></a><span data-ttu-id="1fa53-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="1fa53-103">Create personAward</span></span>

<span data-ttu-id="1fa53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fa53-105">Создание объекта [personAward](../resources/personaward.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa53-105">Create a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa53-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa53-106">Permissions</span></span>

<span data-ttu-id="1fa53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fa53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa53-109">Permission type</span></span>                        | <span data-ttu-id="1fa53-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fa53-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1fa53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fa53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fa53-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa53-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1fa53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fa53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa53-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa53-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1fa53-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fa53-115">Application</span></span>                            | <span data-ttu-id="1fa53-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa53-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="1fa53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fa53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a><span data-ttu-id="1fa53-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fa53-118">Request headers</span></span>
|<span data-ttu-id="1fa53-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1fa53-119">Name</span></span>|<span data-ttu-id="1fa53-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa53-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1fa53-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fa53-121">Authorization</span></span>|<span data-ttu-id="1fa53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa53-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1fa53-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fa53-124">Content-Type</span></span>|<span data-ttu-id="1fa53-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa53-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fa53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fa53-127">Request body</span></span>
<span data-ttu-id="1fa53-128">Представьте в тексте запроса описание объекта [personAward в формате](../resources/personaward.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="1fa53-128">In the request body, supply a JSON representation of the [personAward](../resources/personaward.md) object.</span></span>

<span data-ttu-id="1fa53-129">В следующей таблице показаны свойства, которые можно установить при создании объекта [personAward](../resources/personaward.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa53-129">The following table shows the properties that are possible to set when creating a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="1fa53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fa53-130">Property</span></span>|<span data-ttu-id="1fa53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa53-131">Type</span></span>|<span data-ttu-id="1fa53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa53-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1fa53-133">allowedAudiences</span></span>|<span data-ttu-id="1fa53-134">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-134">String</span></span>|<span data-ttu-id="1fa53-135">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="1fa53-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1fa53-136">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="1fa53-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1fa53-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1fa53-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1fa53-138">description</span><span class="sxs-lookup"><span data-stu-id="1fa53-138">description</span></span>|<span data-ttu-id="1fa53-139">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-139">String</span></span>|<span data-ttu-id="1fa53-140">Условное пожарние.</span><span class="sxs-lookup"><span data-stu-id="1fa53-140">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="1fa53-141">displayName</span><span class="sxs-lookup"><span data-stu-id="1fa53-141">displayName</span></span>|<span data-ttu-id="1fa53-142">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-142">String</span></span>|<span data-ttu-id="1fa53-143">Имя окончания или снадок.</span><span class="sxs-lookup"><span data-stu-id="1fa53-143">Name of the award or honor.</span></span> |
|<span data-ttu-id="1fa53-144">inference</span><span class="sxs-lookup"><span data-stu-id="1fa53-144">inference</span></span>|[<span data-ttu-id="1fa53-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1fa53-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1fa53-146">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="1fa53-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1fa53-147">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="1fa53-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1fa53-148">issuedDate</span><span class="sxs-lookup"><span data-stu-id="1fa53-148">issuedDate</span></span>|<span data-ttu-id="1fa53-149">Дата</span><span class="sxs-lookup"><span data-stu-id="1fa53-149">Date</span></span>|<span data-ttu-id="1fa53-150">Дата предоставления навыка или света.</span><span class="sxs-lookup"><span data-stu-id="1fa53-150">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="1fa53-151">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="1fa53-151">issuingAuthority</span></span>|<span data-ttu-id="1fa53-152">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-152">String</span></span>|<span data-ttu-id="1fa53-153">Центр, предоставивший навыки или свой.</span><span class="sxs-lookup"><span data-stu-id="1fa53-153">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="1fa53-154">source</span><span class="sxs-lookup"><span data-stu-id="1fa53-154">source</span></span>|[<span data-ttu-id="1fa53-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="1fa53-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1fa53-156">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="1fa53-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="1fa53-157">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="1fa53-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1fa53-158">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="1fa53-158">thumbnailUrl</span></span>|<span data-ttu-id="1fa53-159">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-159">String</span></span>|<span data-ttu-id="1fa53-160">URL-адрес ссылается на эскиз удостоверяющего или свободы.</span><span class="sxs-lookup"><span data-stu-id="1fa53-160">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="1fa53-161">webUrl</span><span class="sxs-lookup"><span data-stu-id="1fa53-161">webUrl</span></span>|<span data-ttu-id="1fa53-162">String</span><span class="sxs-lookup"><span data-stu-id="1fa53-162">String</span></span>|<span data-ttu-id="1fa53-163">URL-адрес ссылаться на удачный или снимок.</span><span class="sxs-lookup"><span data-stu-id="1fa53-163">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="1fa53-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa53-164">Response</span></span>

<span data-ttu-id="1fa53-165">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект personAward](../resources/personaward.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1fa53-165">If successful, this method returns a `201 Created` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fa53-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="1fa53-166">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="1fa53-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa53-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personaward_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/awards
Content-Type: application/json
Content-length: 497

{
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="1fa53-168">C#</span><span class="sxs-lookup"><span data-stu-id="1fa53-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personaward-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fa53-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fa53-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personaward-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fa53-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fa53-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personaward-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1fa53-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa53-171">Response</span></span>
<span data-ttu-id="1fa53-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1fa53-172">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
