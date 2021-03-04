---
title: Создание учетной записи
description: Создайте новый объект учетной записи.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 308f2a1e4087fcbb07efb08be8fc1e4cba7d819f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441026"
---
# <a name="create-account"></a><span data-ttu-id="1ab2e-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="1ab2e-103">Create account</span></span>
<span data-ttu-id="1ab2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ab2e-105">Создание нового [объекта userAccountInformation](../resources/useraccountinformation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ab2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ab2e-106">Permissions</span></span>

<span data-ttu-id="1ab2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ab2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ab2e-109">Permission type</span></span>                        | <span data-ttu-id="1ab2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ab2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ab2e-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab2e-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1ab2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab2e-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab2e-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1ab2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ab2e-115">Application</span></span>                            | <span data-ttu-id="1ab2e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab2e-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1ab2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ab2e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a><span data-ttu-id="1ab2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ab2e-118">Request headers</span></span>
|<span data-ttu-id="1ab2e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1ab2e-119">Name</span></span>|<span data-ttu-id="1ab2e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1ab2e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1ab2e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ab2e-121">Authorization</span></span>|<span data-ttu-id="1ab2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1ab2e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ab2e-124">Content-Type</span></span>|<span data-ttu-id="1ab2e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ab2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ab2e-127">Request body</span></span>
<span data-ttu-id="1ab2e-128">В теле запроса поставляем представление JSON объекта [userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="1ab2e-129">В следующей таблице показаны свойства, необходимые при создании нового [объекта userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="1ab2e-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="1ab2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ab2e-130">Property</span></span>|<span data-ttu-id="1ab2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ab2e-131">Type</span></span>|<span data-ttu-id="1ab2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ab2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ab2e-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1ab2e-133">allowedAudiences</span></span>|<span data-ttu-id="1ab2e-134">String</span><span class="sxs-lookup"><span data-stu-id="1ab2e-134">String</span></span>|<span data-ttu-id="1ab2e-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1ab2e-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1ab2e-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1ab2e-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="1ab2e-138">countryCode</span></span>|<span data-ttu-id="1ab2e-139">String</span><span class="sxs-lookup"><span data-stu-id="1ab2e-139">String</span></span>|<span data-ttu-id="1ab2e-140">Содержит код страны с двумя символами, связанный с учетной записью пользователей.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="1ab2e-141">вывод</span><span class="sxs-lookup"><span data-stu-id="1ab2e-141">inference</span></span>|[<span data-ttu-id="1ab2e-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1ab2e-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1ab2e-143">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1ab2e-144">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1ab2e-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="1ab2e-145">preferredLanguageTag</span></span>|[<span data-ttu-id="1ab2e-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="1ab2e-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="1ab2e-147">Содержит язык, который пользователь связал в качестве предпочтительного для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="1ab2e-148">source</span><span class="sxs-lookup"><span data-stu-id="1ab2e-148">source</span></span>|[<span data-ttu-id="1ab2e-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="1ab2e-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1ab2e-150">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="1ab2e-151">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1ab2e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="1ab2e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ab2e-152">Response</span></span>

<span data-ttu-id="1ab2e-153">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект userAccountInformation](../resources/useraccountinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ab2e-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ab2e-154">Examples</span></span>


# <a name="http"></a>[<span data-ttu-id="1ab2e-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ab2e-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/account
Content-Type: application/json
Content-length: 494

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[<span data-ttu-id="1ab2e-156">C#</span><span class="sxs-lookup"><span data-stu-id="1ab2e-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-useraccountinformation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ab2e-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ab2e-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-useraccountinformation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ab2e-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ab2e-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-useraccountinformation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ab2e-159">Java</span><span class="sxs-lookup"><span data-stu-id="1ab2e-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-useraccountinformation-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ab2e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ab2e-160">Response</span></span>
<span data-ttu-id="1ab2e-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ab2e-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


