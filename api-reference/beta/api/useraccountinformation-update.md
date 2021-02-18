---
title: Обновление userAccountInformation
description: Обновление свойств объекта userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8638eeadd59ba7efaae0e6ad32bd4f740dab6d36
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291995"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="196fe-103">Обновление useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="196fe-103">Update useraccountinformation</span></span>

<span data-ttu-id="196fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="196fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="196fe-105">Обновление свойств объекта [userAccountInformation](../resources/useraccountinformation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="196fe-105">Update the properties of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="196fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="196fe-106">Permissions</span></span>

<span data-ttu-id="196fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="196fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="196fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="196fe-109">Permission type</span></span>                        | <span data-ttu-id="196fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="196fe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="196fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="196fe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="196fe-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196fe-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="196fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="196fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="196fe-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196fe-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="196fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="196fe-115">Application</span></span>                            | <span data-ttu-id="196fe-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196fe-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="196fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="196fe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
PATCH /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="196fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="196fe-118">Request headers</span></span>

| <span data-ttu-id="196fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="196fe-119">Name</span></span>           |<span data-ttu-id="196fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="196fe-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="196fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="196fe-121">Authorization</span></span>  | <span data-ttu-id="196fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="196fe-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="196fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="196fe-124">Content-Type</span></span>   | <span data-ttu-id="196fe-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="196fe-125">application/json.</span></span> <span data-ttu-id="196fe-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="196fe-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="196fe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="196fe-127">Request body</span></span>

<span data-ttu-id="196fe-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="196fe-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="196fe-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="196fe-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="196fe-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="196fe-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="196fe-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="196fe-131">Property</span></span>|<span data-ttu-id="196fe-132">Тип</span><span class="sxs-lookup"><span data-stu-id="196fe-132">Type</span></span>|<span data-ttu-id="196fe-133">Описание</span><span class="sxs-lookup"><span data-stu-id="196fe-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="196fe-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="196fe-134">allowedAudiences</span></span>|<span data-ttu-id="196fe-135">String</span><span class="sxs-lookup"><span data-stu-id="196fe-135">String</span></span>|<span data-ttu-id="196fe-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="196fe-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="196fe-137">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="196fe-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="196fe-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="196fe-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="196fe-139">countryCode</span><span class="sxs-lookup"><span data-stu-id="196fe-139">countryCode</span></span>|<span data-ttu-id="196fe-140">String</span><span class="sxs-lookup"><span data-stu-id="196fe-140">String</span></span>|<span data-ttu-id="196fe-141">Содержит двух символьный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="196fe-141">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="196fe-142">вывод</span><span class="sxs-lookup"><span data-stu-id="196fe-142">inference</span></span>|[<span data-ttu-id="196fe-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="196fe-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="196fe-144">Содержит сведения о выводе, если сущность создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="196fe-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="196fe-145">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="196fe-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="196fe-146">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="196fe-146">preferredLanguageTag</span></span>|[<span data-ttu-id="196fe-147">localeInfo</span><span class="sxs-lookup"><span data-stu-id="196fe-147">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="196fe-148">Содержит язык, который пользователь связал как предпочтительный для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="196fe-148">Contains the language the user has associated as preferred for the account.</span></span>   |

## <a name="response"></a><span data-ttu-id="196fe-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="196fe-149">Response</span></span>

<span data-ttu-id="196fe-150">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userAccountInformation](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="196fe-150">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="196fe-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="196fe-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="196fe-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="196fe-152">Request</span></span>

<span data-ttu-id="196fe-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="196fe-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="196fe-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="196fe-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "countryCode": "NO"
}
```
# <a name="c"></a>[<span data-ttu-id="196fe-155">C#</span><span class="sxs-lookup"><span data-stu-id="196fe-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="196fe-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="196fe-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="196fe-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="196fe-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="196fe-158">Java</span><span class="sxs-lookup"><span data-stu-id="196fe-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="196fe-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="196fe-159">Response</span></span>

<span data-ttu-id="196fe-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="196fe-160">The following is an example of the response.</span></span>

> <span data-ttu-id="196fe-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="196fe-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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


