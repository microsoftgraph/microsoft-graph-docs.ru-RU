---
title: Обновление Усераккаунтинформатион
description: Обновление свойств объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 429e26ef14ed461c61f00072cdad878f59d5870f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451604"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="6e9c4-103">Обновление усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="6e9c4-103">Update useraccountinformation</span></span>

<span data-ttu-id="6e9c4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e9c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e9c4-105">Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-105">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e9c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e9c4-106">Permissions</span></span>

<span data-ttu-id="6e9c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e9c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e9c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e9c4-109">Permission type</span></span>                        | <span data-ttu-id="6e9c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e9c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e9c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e9c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e9c4-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6e9c4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6e9c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e9c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e9c4-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6e9c4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6e9c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e9c4-115">Application</span></span>                            | <span data-ttu-id="6e9c4-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e9c4-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6e9c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e9c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e9c4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e9c4-118">Request headers</span></span>

| <span data-ttu-id="6e9c4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6e9c4-119">Name</span></span>           |<span data-ttu-id="6e9c4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6e9c4-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="6e9c4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e9c4-121">Authorization</span></span>  | <span data-ttu-id="6e9c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e9c4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e9c4-124">Content-Type</span></span>   | <span data-ttu-id="6e9c4-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-125">application/json.</span></span> <span data-ttu-id="6e9c4-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="6e9c4-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e9c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e9c4-127">Request body</span></span>

<span data-ttu-id="6e9c4-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6e9c4-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6e9c4-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e9c4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e9c4-131">Property</span></span>            | <span data-ttu-id="6e9c4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6e9c4-132">Type</span></span>                                    | <span data-ttu-id="6e9c4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6e9c4-133">Description</span></span>                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="6e9c4-134">ageGroup</span><span class="sxs-lookup"><span data-stu-id="6e9c4-134">ageGroup</span></span>             |<span data-ttu-id="6e9c4-135">String</span><span class="sxs-lookup"><span data-stu-id="6e9c4-135">String</span></span>                                   |<span data-ttu-id="6e9c4-136">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-136">Shows the age group of user.</span></span> <span data-ttu-id="6e9c4-137">Допустимые `null`значения `minor`, `notAdult` и `adult`.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-137">Allowed values `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="6e9c4-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-138">Read Only.</span></span> |
|<span data-ttu-id="6e9c4-139">countryCode</span><span class="sxs-lookup"><span data-stu-id="6e9c4-139">countryCode</span></span>          |<span data-ttu-id="6e9c4-140">String</span><span class="sxs-lookup"><span data-stu-id="6e9c4-140">String</span></span>                                   |<span data-ttu-id="6e9c4-141">Содержит два символа countryCode, связанных с учетной записью "Пользователи".</span><span class="sxs-lookup"><span data-stu-id="6e9c4-141">Contains the two-character countryCode associated with the users account.</span></span>                       |
|<span data-ttu-id="6e9c4-142">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="6e9c4-142">preferredLanguageTag</span></span> |[<span data-ttu-id="6e9c4-143">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6e9c4-143">localeInfo</span></span>](../resources/localeinfo.md) |<span data-ttu-id="6e9c4-144">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-144">Contains the language the user has associated as preferred for the account.</span></span>                     |
|<span data-ttu-id="6e9c4-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e9c4-145">userPrincipalName</span></span>    |<span data-ttu-id="6e9c4-146">String</span><span class="sxs-lookup"><span data-stu-id="6e9c4-146">String</span></span>                                   |<span data-ttu-id="6e9c4-147">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-147">The user principal name (UPN) of the user associated with the account.</span></span>                          |

## <a name="response"></a><span data-ttu-id="6e9c4-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e9c4-148">Response</span></span>

<span data-ttu-id="6e9c4-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-149">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e9c4-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e9c4-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e9c4-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e9c4-151">Request</span></span>

<span data-ttu-id="6e9c4-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e9c4-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e9c4-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6e9c4-154">C#</span><span class="sxs-lookup"><span data-stu-id="6e9c4-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e9c4-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e9c4-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e9c4-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e9c4-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e9c4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e9c4-157">Response</span></span>

<span data-ttu-id="6e9c4-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-158">The following is an example of the response.</span></span>

> <span data-ttu-id="6e9c4-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e9c4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update useraccountinformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
