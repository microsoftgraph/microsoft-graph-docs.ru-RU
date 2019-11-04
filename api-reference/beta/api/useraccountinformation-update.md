---
title: Обновление Усераккаунтинформатион
description: Обновление свойств объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78d890a00916c72b8c48e5b41a1c84e1e2e2ffb8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938143"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="66e53-103">Обновление усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="66e53-103">Update useraccountinformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e53-104">Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="66e53-104">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66e53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66e53-105">Permissions</span></span>

<span data-ttu-id="66e53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66e53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66e53-108">Permission type</span></span>                        | <span data-ttu-id="66e53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66e53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66e53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66e53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66e53-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="66e53-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="66e53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66e53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66e53-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="66e53-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="66e53-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66e53-114">Application</span></span>                            | <span data-ttu-id="66e53-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e53-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="66e53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66e53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66e53-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66e53-117">Request headers</span></span>

| <span data-ttu-id="66e53-118">Имя</span><span class="sxs-lookup"><span data-stu-id="66e53-118">Name</span></span>           |<span data-ttu-id="66e53-119">Описание</span><span class="sxs-lookup"><span data-stu-id="66e53-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="66e53-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66e53-120">Authorization</span></span>  | <span data-ttu-id="66e53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66e53-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="66e53-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66e53-123">Content-Type</span></span>   | <span data-ttu-id="66e53-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="66e53-124">application/json.</span></span> <span data-ttu-id="66e53-125">Обязательное</span><span class="sxs-lookup"><span data-stu-id="66e53-125">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="66e53-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66e53-126">Request body</span></span>

<span data-ttu-id="66e53-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="66e53-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="66e53-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="66e53-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="66e53-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="66e53-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="66e53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e53-130">Property</span></span>            | <span data-ttu-id="66e53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66e53-131">Type</span></span>                                    | <span data-ttu-id="66e53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66e53-132">Description</span></span>                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="66e53-133">ageGroup</span><span class="sxs-lookup"><span data-stu-id="66e53-133">ageGroup</span></span>             |<span data-ttu-id="66e53-134">String</span><span class="sxs-lookup"><span data-stu-id="66e53-134">String</span></span>                                   |<span data-ttu-id="66e53-135">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66e53-135">Shows the age group of user.</span></span> <span data-ttu-id="66e53-136">Допустимые `null`значения `minor`, `notAdult` и `adult`.</span><span class="sxs-lookup"><span data-stu-id="66e53-136">Allowed values `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="66e53-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66e53-137">Read Only.</span></span> |
|<span data-ttu-id="66e53-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="66e53-138">countryCode</span></span>          |<span data-ttu-id="66e53-139">Строка</span><span class="sxs-lookup"><span data-stu-id="66e53-139">String</span></span>                                   |<span data-ttu-id="66e53-140">Содержит два символа countryCode, связанных с учетной записью "Пользователи".</span><span class="sxs-lookup"><span data-stu-id="66e53-140">Contains the two-character countryCode associated with the users account.</span></span>                       |
|<span data-ttu-id="66e53-141">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="66e53-141">preferredLanguageTag</span></span> |[<span data-ttu-id="66e53-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="66e53-142">localeInfo</span></span>](../resources/localeinfo.md) |<span data-ttu-id="66e53-143">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="66e53-143">Contains the language the user has associated as preferred for the account.</span></span>                     |
|<span data-ttu-id="66e53-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66e53-144">userPrincipalName</span></span>    |<span data-ttu-id="66e53-145">String</span><span class="sxs-lookup"><span data-stu-id="66e53-145">String</span></span>                                   |<span data-ttu-id="66e53-146">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="66e53-146">The user principal name (UPN) of the user associated with the account.</span></span>                          |

## <a name="response"></a><span data-ttu-id="66e53-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e53-147">Response</span></span>

<span data-ttu-id="66e53-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66e53-148">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66e53-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="66e53-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66e53-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="66e53-150">Request</span></span>

<span data-ttu-id="66e53-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66e53-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66e53-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e53-152">Response</span></span>

<span data-ttu-id="66e53-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66e53-153">The following is an example of the response.</span></span>

> <span data-ttu-id="66e53-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66e53-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
