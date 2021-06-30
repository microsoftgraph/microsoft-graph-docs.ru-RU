---
title: Обновление userInsightsSettings
description: Обновление свойств объекта userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: a422a106d1371e8e39fdfa314658b8e77d0f5a9a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210667"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="6e747-103">Обновление userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="6e747-103">Update userInsightsSettings</span></span>

<span data-ttu-id="6e747-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e747-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e747-105">Обновим параметры конфиденциальности [для itemInsights и](../resources/iteminsights.md) [сведения](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) о часах собраний пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e747-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e747-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e747-106">Permissions</span></span>

<span data-ttu-id="6e747-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e747-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e747-109">Permission type</span></span>      | <span data-ttu-id="6e747-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e747-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e747-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e747-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e747-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e747-112">User.ReadWrite</span></span> |
|<span data-ttu-id="6e747-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e747-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e747-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e747-114">Not supported.</span></span>    |
|<span data-ttu-id="6e747-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e747-115">Application</span></span> | <span data-ttu-id="6e747-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e747-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6e747-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e747-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="6e747-118">**Примечание:** Запросы с `userId` разрешениями User.ReadWrite.All доступны только пользователю или `userPrincipalName` пользователю.</span><span class="sxs-lookup"><span data-stu-id="6e747-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="6e747-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e747-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e747-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e747-120">Request headers</span></span>

| <span data-ttu-id="6e747-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e747-121">Header</span></span>       | <span data-ttu-id="6e747-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e747-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6e747-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e747-123">Authorization</span></span>  | <span data-ttu-id="6e747-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e747-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e747-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e747-126">Content-Type</span></span>  | <span data-ttu-id="6e747-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e747-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e747-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e747-129">Request body</span></span>

<span data-ttu-id="6e747-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6e747-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e747-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e747-133">Property</span></span>     | <span data-ttu-id="6e747-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6e747-134">Type</span></span>   |<span data-ttu-id="6e747-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6e747-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e747-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6e747-136">isEnabled</span></span>|<span data-ttu-id="6e747-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e747-137">Boolean</span></span>| <span data-ttu-id="6e747-138">`true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены.</span><span class="sxs-lookup"><span data-stu-id="6e747-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="6e747-139">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="6e747-139">Default is `true`.</span></span> <span data-ttu-id="6e747-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6e747-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="6e747-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e747-141">Response</span></span>

<span data-ttu-id="6e747-142">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userInsightsSettings](../resources/userinsightssettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6e747-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e747-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6e747-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="6e747-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e747-144">Request</span></span>

<span data-ttu-id="6e747-145">Ниже приводится пример запроса на то, как пользователь обновляет "**isEnabled**" параметр конфиденциальности, чтобы отключить его сведения о элементе и сведения о часах собраний.</span><span class="sxs-lookup"><span data-stu-id="6e747-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e747-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e747-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6e747-147">C#</span><span class="sxs-lookup"><span data-stu-id="6e747-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e747-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e747-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e747-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e747-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e747-150">Java</span><span class="sxs-lookup"><span data-stu-id="6e747-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6e747-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e747-151">Response</span></span>

<span data-ttu-id="6e747-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6e747-152">The following is an example of the response.</span></span> 

><span data-ttu-id="6e747-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6e747-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
