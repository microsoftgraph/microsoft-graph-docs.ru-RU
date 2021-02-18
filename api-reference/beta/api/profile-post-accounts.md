---
title: Создание учетной записи
description: Создание объекта учетной записи.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d1fb13f513450515361f2bdb15ebfd7461635e1c
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292975"
---
# <a name="create-account"></a><span data-ttu-id="941ad-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="941ad-103">Create account</span></span>
<span data-ttu-id="941ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="941ad-105">Создание объекта [userAccountInformation](../resources/useraccountinformation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="941ad-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="941ad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="941ad-106">Permissions</span></span>

<span data-ttu-id="941ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="941ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941ad-109">Permission type</span></span>                        | <span data-ttu-id="941ad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="941ad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="941ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="941ad-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941ad-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="941ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941ad-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941ad-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="941ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941ad-115">Application</span></span>                            | <span data-ttu-id="941ad-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941ad-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="941ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a><span data-ttu-id="941ad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941ad-118">Request headers</span></span>
|<span data-ttu-id="941ad-119">Имя</span><span class="sxs-lookup"><span data-stu-id="941ad-119">Name</span></span>|<span data-ttu-id="941ad-120">Описание</span><span class="sxs-lookup"><span data-stu-id="941ad-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="941ad-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941ad-121">Authorization</span></span>|<span data-ttu-id="941ad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941ad-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="941ad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="941ad-124">Content-Type</span></span>|<span data-ttu-id="941ad-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941ad-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="941ad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="941ad-127">Request body</span></span>
<span data-ttu-id="941ad-128">В теле запроса укажу представление объекта [userAccountInformation](../resources/useraccountinformation.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="941ad-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="941ad-129">В следующей таблице показаны свойства, необходимые при создании объекта [userAccountInformation.](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="941ad-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="941ad-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="941ad-130">Property</span></span>|<span data-ttu-id="941ad-131">Тип</span><span class="sxs-lookup"><span data-stu-id="941ad-131">Type</span></span>|<span data-ttu-id="941ad-132">Описание</span><span class="sxs-lookup"><span data-stu-id="941ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="941ad-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="941ad-133">allowedAudiences</span></span>|<span data-ttu-id="941ad-134">String</span><span class="sxs-lookup"><span data-stu-id="941ad-134">String</span></span>|<span data-ttu-id="941ad-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="941ad-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="941ad-136">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="941ad-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="941ad-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="941ad-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="941ad-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="941ad-138">countryCode</span></span>|<span data-ttu-id="941ad-139">String</span><span class="sxs-lookup"><span data-stu-id="941ad-139">String</span></span>|<span data-ttu-id="941ad-140">Содержит двух символьный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="941ad-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="941ad-141">вывод</span><span class="sxs-lookup"><span data-stu-id="941ad-141">inference</span></span>|[<span data-ttu-id="941ad-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="941ad-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="941ad-143">Содержит сведения о выводе, если сущность создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="941ad-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="941ad-144">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="941ad-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="941ad-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="941ad-145">preferredLanguageTag</span></span>|[<span data-ttu-id="941ad-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="941ad-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="941ad-147">Содержит язык, который пользователь связал как предпочтительный для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="941ad-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="941ad-148">source</span><span class="sxs-lookup"><span data-stu-id="941ad-148">source</span></span>|[<span data-ttu-id="941ad-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="941ad-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="941ad-150">Где значения возникают, если синхронизированы из другой службы.</span><span class="sxs-lookup"><span data-stu-id="941ad-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="941ad-151">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="941ad-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="941ad-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="941ad-152">Response</span></span>

<span data-ttu-id="941ad-153">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userAccountInformation](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="941ad-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="941ad-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="941ad-154">Examples</span></span>

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

### <a name="response"></a><span data-ttu-id="941ad-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="941ad-155">Response</span></span>
<span data-ttu-id="941ad-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="941ad-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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


