---
title: Get userInsightsSettings
description: Извлечение свойств объекта userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d3d9f370318f74f3c25b8737de4cecc7dbb37d6d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210359"
---
# <a name="get-userinsightssettings"></a><span data-ttu-id="452d4-103">Get userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="452d4-103">Get userInsightsSettings</span></span>

<span data-ttu-id="452d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="452d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="452d4-105">Получите настраиваемые пользователем параметры конфиденциальности для [itemInsights](../resources/iteminsights.md) и сведения [о часах собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="452d4-105">Get the user-customizable privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span>

## <a name="permissions"></a><span data-ttu-id="452d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="452d4-106">Permissions</span></span>

<span data-ttu-id="452d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="452d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="452d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="452d4-109">Permission type</span></span>      | <span data-ttu-id="452d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="452d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="452d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="452d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="452d4-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="452d4-112">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="452d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="452d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="452d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452d4-114">Not supported.</span></span>    |
|<span data-ttu-id="452d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="452d4-115">Application</span></span> | <span data-ttu-id="452d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452d4-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="452d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="452d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

><span data-ttu-id="452d4-118">**Примечание:** Запросы с `userId` разрешениями User.ReadWrite.All доступны только пользователю или `userPrincipalName` пользователю.</span><span class="sxs-lookup"><span data-stu-id="452d4-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="452d4-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="452d4-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="452d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="452d4-120">Request headers</span></span>

| <span data-ttu-id="452d4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="452d4-121">Name</span></span>       | <span data-ttu-id="452d4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="452d4-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="452d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="452d4-123">Authorization</span></span>  | <span data-ttu-id="452d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="452d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="452d4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="452d4-126">Request body</span></span>

<span data-ttu-id="452d4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="452d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="452d4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="452d4-128">Response</span></span>

<span data-ttu-id="452d4-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userInsightsSettings](../resources/userinsightssettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="452d4-129">If successful, this method returns a `200 OK` response code and a [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="452d4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="452d4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="452d4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="452d4-131">Request</span></span>

<span data-ttu-id="452d4-132">Ниже приводится пример запроса на представление элементов пользователя и параметры времени собраний.</span><span class="sxs-lookup"><span data-stu-id="452d4-132">The following is an example of the request to get user item insights and meeting hours insights settings.</span></span>


# <a name="http"></a>[<span data-ttu-id="452d4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="452d4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="452d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="452d4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="452d4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="452d4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="452d4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="452d4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="452d4-137">Java</span><span class="sxs-lookup"><span data-stu-id="452d4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="452d4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="452d4-138">Response</span></span>

<span data-ttu-id="452d4-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="452d4-139">The following is an example of the response.</span></span> 
> <span data-ttu-id="452d4-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="452d4-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "get_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": true
}
```


