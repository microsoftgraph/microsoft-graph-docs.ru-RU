---
title: Создание рабочей силыИнтеграция
description: Создание нового объекта workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76cb01efb15f7937c9e71e1fa26eb8d425f2b4d7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054688"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="067dc-103">Создание рабочей силыИнтеграция</span><span class="sxs-lookup"><span data-stu-id="067dc-103">Create workforceIntegration</span></span>

<span data-ttu-id="067dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="067dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="067dc-105">Создание нового [объекта workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="067dc-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="067dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="067dc-106">Permissions</span></span>

<span data-ttu-id="067dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="067dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="067dc-109">Permission type</span></span>                        | <span data-ttu-id="067dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="067dc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="067dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="067dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="067dc-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067dc-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="067dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="067dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="067dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067dc-114">Not supported.</span></span> |
| <span data-ttu-id="067dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="067dc-115">Application</span></span>                            | <span data-ttu-id="067dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067dc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="067dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="067dc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="067dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="067dc-118">Request headers</span></span>

| <span data-ttu-id="067dc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="067dc-119">Name</span></span>          | <span data-ttu-id="067dc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="067dc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="067dc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="067dc-121">Authorization</span></span> | <span data-ttu-id="067dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="067dc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="067dc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="067dc-124">Content-type</span></span> | <span data-ttu-id="067dc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="067dc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="067dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="067dc-127">Request body</span></span>

<span data-ttu-id="067dc-128">В теле запроса поставляем представление JSON объекта [workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="067dc-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="067dc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="067dc-129">Response</span></span>

<span data-ttu-id="067dc-130">В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="067dc-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="067dc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="067dc-131">Examples</span></span>

### <a name="example-1-create-a-new-workforceintegration-object"></a><span data-ttu-id="067dc-132">Пример 1. Создание нового объекта workforceIntegration.</span><span class="sxs-lookup"><span data-stu-id="067dc-132">Example 1: Create a new workforceIntegration object.</span></span>

#### <a name="request"></a><span data-ttu-id="067dc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="067dc-133">Request</span></span>

<span data-ttu-id="067dc-134">Ниже приводится пример запроса на создание нового объекта **workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="067dc-134">The following is an example of a request to create a new **workforceIntegration** object.</span></span>

# <a name="http"></a>[<span data-ttu-id="067dc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="067dc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[<span data-ttu-id="067dc-136">C#</span><span class="sxs-lookup"><span data-stu-id="067dc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="067dc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="067dc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="067dc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="067dc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="067dc-139">Java</span><span class="sxs-lookup"><span data-stu-id="067dc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="067dc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="067dc-140">Response</span></span>

<span data-ttu-id="067dc-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="067dc-141">The following is an example of the response.</span></span>

> <span data-ttu-id="067dc-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="067dc-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="067dc-143">Пример 2. Создание новой рабочей силыИнтеграция с помощью SwapRequest, включенной для фильтрации прав</span><span class="sxs-lookup"><span data-stu-id="067dc-143">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="067dc-144">Ниже приводится пример запроса с помощью SwapRequest, включенного для фильтрации прав.</span><span class="sxs-lookup"><span data-stu-id="067dc-144">The following is an example of a request with SwapRequest enabled for eligibility filtering.</span></span> 

#### <a name="request"></a><span data-ttu-id="067dc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="067dc-145">Request</span></span>

```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a><span data-ttu-id="067dc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="067dc-146">Response</span></span>

<span data-ttu-id="067dc-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="067dc-147">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
<span data-ttu-id="067dc-148">Чтобы обновить существующий **объект workforceIntegration** с помощью swapRequest, включенного для фильтрации прав, см. в [методе Update.](../api/workforceintegration-update.md)</span><span class="sxs-lookup"><span data-stu-id="067dc-148">To update an existing **workforceIntegration** object with SwapRequest enabled for eligibility filtering, see the [Update](../api/workforceintegration-update.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="067dc-149">Пример 3. Получение подходящих сдвигов при включении SwapRequest в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="067dc-149">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="067dc-150">Взаимодействие между конечными точками интеграции shifts и рабочей силой будет следовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="067dc-150">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="067dc-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="067dc-151">Request</span></span>

<span data-ttu-id="067dc-152">Ниже приводится пример запроса shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span><span class="sxs-lookup"><span data-stu-id="067dc-152">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
### <a name="response"></a><span data-ttu-id="067dc-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="067dc-153">Response</span></span>

<span data-ttu-id="067dc-154">Ниже приводится пример ответа службы интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="067dc-154">The following is an example of the response from the workforce integration service.</span></span>
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


