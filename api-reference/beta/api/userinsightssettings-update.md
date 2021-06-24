---
title: Обновление userInsightsSettings
description: Обновление свойств объекта userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5f161d5b75e862f358d07fee2347bb3f4d18bbad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107912"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="a6cd7-103">Обновление userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="a6cd7-103">Update userInsightsSettings</span></span>

<span data-ttu-id="a6cd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6cd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6cd7-105">Обновим параметры конфиденциальности [для itemInsights и](../resources/iteminsights.md) [сведения](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) о часах собраний пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6cd7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6cd7-106">Permissions</span></span>

<span data-ttu-id="a6cd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6cd7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6cd7-109">Permission type</span></span>      | <span data-ttu-id="a6cd7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6cd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6cd7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6cd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6cd7-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6cd7-112">User.ReadWrite</span></span> |
|<span data-ttu-id="a6cd7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6cd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6cd7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-114">Not supported.</span></span>    |
|<span data-ttu-id="a6cd7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6cd7-115">Application</span></span> | <span data-ttu-id="a6cd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a6cd7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6cd7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="a6cd7-118">**Примечание:** Запросы с `userId` разрешениями User.ReadWrite.All доступны только пользователю или `userPrincipalName` пользователю.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="a6cd7-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6cd7-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6cd7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6cd7-120">Request headers</span></span>

| <span data-ttu-id="a6cd7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6cd7-121">Header</span></span>       | <span data-ttu-id="a6cd7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a6cd7-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a6cd7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6cd7-123">Authorization</span></span>  | <span data-ttu-id="a6cd7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a6cd7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6cd7-126">Content-Type</span></span>  | <span data-ttu-id="a6cd7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6cd7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6cd7-129">Request body</span></span>

<span data-ttu-id="a6cd7-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6cd7-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6cd7-133">Property</span></span>     | <span data-ttu-id="a6cd7-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a6cd7-134">Type</span></span>   |<span data-ttu-id="a6cd7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a6cd7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6cd7-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a6cd7-136">isEnabled</span></span>|<span data-ttu-id="a6cd7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6cd7-137">Boolean</span></span>| <span data-ttu-id="a6cd7-138">`true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="a6cd7-139">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-139">Default is `true`.</span></span> <span data-ttu-id="a6cd7-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="a6cd7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6cd7-141">Response</span></span>

<span data-ttu-id="a6cd7-142">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userInsightsSettings](../resources/userinsightssettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6cd7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="a6cd7-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="a6cd7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6cd7-144">Request</span></span>

<span data-ttu-id="a6cd7-145">Ниже приводится пример запроса на то, как пользователь обновляет "**isEnabled**" параметр конфиденциальности, чтобы отключить его сведения о элементе и сведения о часах собраний.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userInsightsSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{userId}/settings/itemInsights
Content-type: application/json

{
  "isEnabled": "false"
}
```


### <a name="response"></a><span data-ttu-id="a6cd7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6cd7-146">Response</span></span>

<span data-ttu-id="a6cd7-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-147">The following is an example of the response.</span></span> 

><span data-ttu-id="a6cd7-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a6cd7-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "update_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": false,
}
```
