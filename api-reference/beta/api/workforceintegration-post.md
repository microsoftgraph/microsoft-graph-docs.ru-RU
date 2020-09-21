---
title: Создание Воркфорцеинтегратион
description: Создание нового объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e7640b781c15f19d9ee15883d715c99243cbd5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989768"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="020ee-103">Создание Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="020ee-103">Create workforceIntegration</span></span>

<span data-ttu-id="020ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="020ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="020ee-105">Создание нового объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="020ee-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="020ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="020ee-106">Permissions</span></span>

<span data-ttu-id="020ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="020ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="020ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="020ee-109">Permission type</span></span>                        | <span data-ttu-id="020ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="020ee-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="020ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="020ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="020ee-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="020ee-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="020ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="020ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="020ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020ee-114">Not supported.</span></span> |
| <span data-ttu-id="020ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="020ee-115">Application</span></span>                            | <span data-ttu-id="020ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020ee-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="020ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="020ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="020ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="020ee-118">Request headers</span></span>

| <span data-ttu-id="020ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="020ee-119">Name</span></span>          | <span data-ttu-id="020ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="020ee-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="020ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="020ee-121">Authorization</span></span> | <span data-ttu-id="020ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="020ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="020ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="020ee-124">Content-type</span></span> | <span data-ttu-id="020ee-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="020ee-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="020ee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="020ee-127">Request body</span></span>

<span data-ttu-id="020ee-128">В тексте запроса добавьте представление объекта [воркфорцеинтегратион](../resources/workforceintegration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="020ee-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="020ee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="020ee-129">Response</span></span>

<span data-ttu-id="020ee-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="020ee-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="020ee-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="020ee-131">Examples</span></span>

### <a name="example-1-create-a-new-workforceintegration-object"></a><span data-ttu-id="020ee-132">Пример 1: создание нового объекта Воркфорцеинтегратион.</span><span class="sxs-lookup"><span data-stu-id="020ee-132">Example 1: Create a new workforceIntegration object.</span></span>

#### <a name="request"></a><span data-ttu-id="020ee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="020ee-133">Request</span></span>

<span data-ttu-id="020ee-134">Ниже приведен пример запроса на создание нового объекта **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="020ee-134">The following is an example of a request to create a new **workforceIntegration** object.</span></span>

# <a name="http"></a>[<span data-ttu-id="020ee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="020ee-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="020ee-136">C#</span><span class="sxs-lookup"><span data-stu-id="020ee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="020ee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="020ee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="020ee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="020ee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="020ee-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="020ee-139">Response</span></span>

<span data-ttu-id="020ee-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="020ee-140">The following is an example of the response.</span></span>

> <span data-ttu-id="020ee-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="020ee-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="020ee-143">Пример 2: создание нового Воркфорцеинтегратион с включенной функцией Свапрекуест для фильтрации допустимости</span><span class="sxs-lookup"><span data-stu-id="020ee-143">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="020ee-144">Ниже приведен пример запроса с Свапрекуест, включенным для фильтрации приемлемости.</span><span class="sxs-lookup"><span data-stu-id="020ee-144">The following is an example of a request with SwapRequest enabled for eligibility filtering.</span></span> 

#### <a name="request"></a><span data-ttu-id="020ee-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="020ee-145">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="020ee-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="020ee-146">Response</span></span>

<span data-ttu-id="020ee-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="020ee-147">The following is an example of the response.</span></span>
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
<span data-ttu-id="020ee-148">Чтобы обновить существующий объект **воркфорцеинтегратион** с свапрекуест, включенным для фильтрации допустимости, ознакомьтесь со статьей метод [Update](../api/workforceintegration-update.md) .</span><span class="sxs-lookup"><span data-stu-id="020ee-148">To update an existing **workforceIntegration** object with SwapRequest enabled for eligibility filtering, see the [Update](../api/workforceintegration-update.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="020ee-149">Пример 3: получение подходящих смен при включении Свапрекуест в Елигибилитифилтеринженабледентитиес</span><span class="sxs-lookup"><span data-stu-id="020ee-149">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="020ee-150">Конечные точки интеграции "взаимодействие между сменами приложения" и "ресурсы" будут соответствовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="020ee-150">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="020ee-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="020ee-151">Request</span></span>

<span data-ttu-id="020ee-152">Ниже приведен пример запроса, сделанного сменам конечной точки интеграции сотрудников для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="020ee-152">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="020ee-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="020ee-153">Response</span></span>

<span data-ttu-id="020ee-154">Ниже приведен пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="020ee-154">The following is an example of the response from the workforce integration service.</span></span>
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


