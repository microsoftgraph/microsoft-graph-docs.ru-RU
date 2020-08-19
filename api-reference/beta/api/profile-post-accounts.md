---
title: Создание учетной записи
description: Создайте новый объект Account.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 67e77365f4ad46a48aac49ba8733093df5a758ce
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813138"
---
# <a name="create-account"></a><span data-ttu-id="70130-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="70130-103">Create account</span></span>
<span data-ttu-id="70130-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70130-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70130-105">Создание нового объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="70130-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="70130-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70130-106">Permissions</span></span>

<span data-ttu-id="70130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70130-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70130-109">Permission type</span></span>                        | <span data-ttu-id="70130-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70130-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="70130-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70130-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70130-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70130-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="70130-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70130-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70130-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70130-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="70130-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70130-115">Application</span></span>                            | <span data-ttu-id="70130-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70130-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="70130-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70130-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/accounts
POST /users/{id | userPrincipalName}/profile/accounts
```

## <a name="request-headers"></a><span data-ttu-id="70130-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70130-118">Request headers</span></span>
|<span data-ttu-id="70130-119">Имя</span><span class="sxs-lookup"><span data-stu-id="70130-119">Name</span></span>|<span data-ttu-id="70130-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70130-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70130-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70130-121">Authorization</span></span>|<span data-ttu-id="70130-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70130-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="70130-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70130-124">Content-Type</span></span>|<span data-ttu-id="70130-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70130-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70130-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70130-127">Request body</span></span>
<span data-ttu-id="70130-128">В тексте запроса добавьте представление объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70130-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="70130-129">В следующей таблице приведены свойства, необходимые при создании нового объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="70130-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="70130-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="70130-130">Property</span></span>|<span data-ttu-id="70130-131">Тип</span><span class="sxs-lookup"><span data-stu-id="70130-131">Type</span></span>|<span data-ttu-id="70130-132">Описание</span><span class="sxs-lookup"><span data-stu-id="70130-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70130-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="70130-133">allowedAudiences</span></span>|<span data-ttu-id="70130-134">String</span><span class="sxs-lookup"><span data-stu-id="70130-134">String</span></span>|<span data-ttu-id="70130-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="70130-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="70130-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="70130-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="70130-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="70130-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="70130-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="70130-138">countryCode</span></span>|<span data-ttu-id="70130-139">String</span><span class="sxs-lookup"><span data-stu-id="70130-139">String</span></span>|<span data-ttu-id="70130-140">Содержит двухбуквенный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="70130-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="70130-141">выводов</span><span class="sxs-lookup"><span data-stu-id="70130-141">inference</span></span>|[<span data-ttu-id="70130-142">инференцедата</span><span class="sxs-lookup"><span data-stu-id="70130-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="70130-143">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="70130-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="70130-144">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="70130-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="70130-145">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="70130-145">preferredLanguageTag</span></span>|[<span data-ttu-id="70130-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="70130-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="70130-147">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="70130-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="70130-148">source</span><span class="sxs-lookup"><span data-stu-id="70130-148">source</span></span>|[<span data-ttu-id="70130-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="70130-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="70130-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="70130-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="70130-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="70130-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="70130-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="70130-152">Response</span></span>

<span data-ttu-id="70130-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70130-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70130-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="70130-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="70130-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="70130-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/accounts
Content-Type: application/json
Content-length: 494

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[<span data-ttu-id="70130-156">C#</span><span class="sxs-lookup"><span data-stu-id="70130-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70130-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70130-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70130-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70130-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="70130-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="70130-159">Response</span></span>
<span data-ttu-id="70130-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70130-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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
