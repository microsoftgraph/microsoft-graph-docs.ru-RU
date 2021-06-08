---
title: Обновление реинтеграции рабочей силы
description: Обновление свойств объекта по реинтеграции рабочей силы.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c62a27e7c0a019023bea7549523dc8b9de7582c1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787998"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="b671d-103">Обновление реинтеграции рабочей силы</span><span class="sxs-lookup"><span data-stu-id="b671d-103">Update workforceintegration</span></span>

<span data-ttu-id="b671d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b671d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b671d-105">Обновление свойств объекта [по реинтеграции](../resources/workforceintegration.md) рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="b671d-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b671d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b671d-106">Permissions</span></span>

<span data-ttu-id="b671d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b671d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b671d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b671d-109">Permission type</span></span>                        | <span data-ttu-id="b671d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b671d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b671d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b671d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b671d-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b671d-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b671d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b671d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b671d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b671d-114">Not supported.</span></span> |
| <span data-ttu-id="b671d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b671d-115">Application</span></span>                            | <span data-ttu-id="b671d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b671d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b671d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b671d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="b671d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b671d-118">Request headers</span></span>

| <span data-ttu-id="b671d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b671d-119">Name</span></span>       | <span data-ttu-id="b671d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b671d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b671d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b671d-121">Authorization</span></span> | <span data-ttu-id="b671d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b671d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b671d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b671d-123">Request body</span></span>

<span data-ttu-id="b671d-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b671d-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b671d-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b671d-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b671d-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b671d-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b671d-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="b671d-127">Property</span></span>     | <span data-ttu-id="b671d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b671d-128">Type</span></span>        | <span data-ttu-id="b671d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b671d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b671d-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="b671d-130">apiVersion</span></span>|<span data-ttu-id="b671d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b671d-131">Int32</span></span>|<span data-ttu-id="b671d-132">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="b671d-132">API version for the call back url.</span></span> <span data-ttu-id="b671d-133">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="b671d-133">Start with 1.</span></span>|
|<span data-ttu-id="b671d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b671d-134">displayName</span></span>|<span data-ttu-id="b671d-135">String</span><span class="sxs-lookup"><span data-stu-id="b671d-135">String</span></span>|<span data-ttu-id="b671d-136">Имя интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="b671d-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="b671d-137">шифрование</span><span class="sxs-lookup"><span data-stu-id="b671d-137">encryption</span></span>|<span data-ttu-id="b671d-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="b671d-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="b671d-139">Ресурс шифрования интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="b671d-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="b671d-140">isActive</span><span class="sxs-lookup"><span data-stu-id="b671d-140">isActive</span></span>|<span data-ttu-id="b671d-141">Логический</span><span class="sxs-lookup"><span data-stu-id="b671d-141">Boolean</span></span>|<span data-ttu-id="b671d-142">Указывает, является ли эта интеграция рабочей силы активной и доступной в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="b671d-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="b671d-143">поддерживает</span><span class="sxs-lookup"><span data-stu-id="b671d-143">supports</span></span>|<span data-ttu-id="b671d-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b671d-144">string</span></span>| <span data-ttu-id="b671d-145">Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="b671d-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="b671d-146">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.</span><span class="sxs-lookup"><span data-stu-id="b671d-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="b671d-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="b671d-147">supportedEntities</span></span>|<span data-ttu-id="b671d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b671d-148">string</span></span>| <span data-ttu-id="b671d-149">Это свойство заменит **поддержки** в v1.0.</span><span class="sxs-lookup"><span data-stu-id="b671d-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="b671d-150">Рекомендуется использовать это свойство вместо **поддержки.**</span><span class="sxs-lookup"><span data-stu-id="b671d-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="b671d-151">Свойство **поддерживается** в бета-версии в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="b671d-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="b671d-152">Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="b671d-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="b671d-153">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.</span><span class="sxs-lookup"><span data-stu-id="b671d-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="b671d-154">url</span><span class="sxs-lookup"><span data-stu-id="b671d-154">url</span></span>|<span data-ttu-id="b671d-155">String</span><span class="sxs-lookup"><span data-stu-id="b671d-155">String</span></span>| <span data-ttu-id="b671d-156">URL-адрес интеграции рабочей силы для вызовов из службы Shift.</span><span class="sxs-lookup"><span data-stu-id="b671d-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="b671d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="b671d-157">Response</span></span>

<span data-ttu-id="b671d-158">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b671d-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b671d-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="b671d-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="b671d-160">Пример 1. Обновление объекта workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b671d-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="b671d-161">В следующем примере обновляется **объект workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="b671d-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="b671d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="b671d-162">Request</span></span>

<span data-ttu-id="b671d-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b671d-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b671d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b671d-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
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
# <a name="c"></a>[<span data-ttu-id="b671d-165">C#</span><span class="sxs-lookup"><span data-stu-id="b671d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b671d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b671d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b671d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b671d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b671d-168">Java</span><span class="sxs-lookup"><span data-stu-id="b671d-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b671d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b671d-169">Response</span></span>

<span data-ttu-id="b671d-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b671d-170">The following is an example of the response.</span></span>

> <span data-ttu-id="b671d-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b671d-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="b671d-172">Пример 2. Создание новой рабочей силыИнтеграция с помощью SwapRequest, включенной для фильтрации прав</span><span class="sxs-lookup"><span data-stu-id="b671d-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="b671d-173">В следующем примере создается новая **рабочая силаИнтеграция** с поддержкой SwapRequest для фильтрации прав.</span><span class="sxs-lookup"><span data-stu-id="b671d-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="b671d-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="b671d-174">Request</span></span>

<span data-ttu-id="b671d-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b671d-175">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="b671d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="b671d-176">Response</span></span>

<span data-ttu-id="b671d-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b671d-177">The following is an example of the response.</span></span>
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
<span data-ttu-id="b671d-178">Чтобы создать новую **рабочую силуИнтеграция** с помощью SwapRequest, включенной для фильтрации прав, см. в [методе Create.](../api/workforceintegration-post.md)</span><span class="sxs-lookup"><span data-stu-id="b671d-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="b671d-179">Пример 3. Получение подходящих сдвигов при включении SwapRequest в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="b671d-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="b671d-180">Взаимодействие между конечными точками интеграции shifts и рабочей силой будет следовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="b671d-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="b671d-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="b671d-181">Request</span></span>

<span data-ttu-id="b671d-182">Ниже приводится пример запроса shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span><span class="sxs-lookup"><span data-stu-id="b671d-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="b671d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="b671d-183">Response</span></span>

<span data-ttu-id="b671d-184">Ниже приводится пример ответа службы интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="b671d-184">The following is an example of the response from the workforce integration service.</span></span>
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

### <a name="example-4-shifts-synchronous-call-back-to-the-workforce-integration-endpoint-when-enabled-for-real-time-notifications-on-timecard-changes"></a><span data-ttu-id="b671d-185">Пример 4. Перенос синхронного вызова обратно в конечную точку интеграции рабочей силы при включении уведомлений в режиме реального времени при изменениях timeCard.</span><span class="sxs-lookup"><span data-stu-id="b671d-185">Example 4: Shifts synchronous call back to the workforce integration endpoint when enabled for real time notifications on timeCard changes.</span></span>

#### <a name="request"></a><span data-ttu-id="b671d-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="b671d-186">Request</span></span>

<span data-ttu-id="b671d-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b671d-187">The following is an example of the request.</span></span> 
```
POST https://foobarWorkforceIntegration.com/foobar/v1/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/update
Accept-Language: en-us
X-MS-WFMPassthrough: foobarvalue
Content-type: application/json
{
   "requests":[
      {
         "id":"1",
         "method":"POST",
         "url":"/timecards",
         "headers":{
            "X-MS-Transaction-ID":"1"
         },
         "body":{
            "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
            "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
            "createdDateTime":"2019-03-18T00:00:00.000Z",
            "createdBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
            "lastModifiedBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "state":"onBreak",
            "clockIn":{
               "dateTime":"2019-03-18T00:00:00.000Z",
               "atApprovedLocation":true,
               "notes":null
            },
            "clockOut":null,
            "breaks":[
               {
                  "id":"string",
                  "notes":{
                     "content":"Lunch break",
                     "contentType":"text"
                  },
                  "start":{
                     "dateTime":"2019-03-18T00:00:00.000Z",
                     "atApprovedLocation":true,
                     "notes":{
                        "content":"Started my break 5 minutes early",
                        "contentType":"text"
                     }
                  },
                  "end":null
               }
            ],
            "notes":null,
            "originalEntry":{
               "clockIn":{
                  "dateTime":"2019-03-18T00:00:00.000Z",
                  "atApprovedLocation":true,
                  "notes":null
               },
               "clockOut":null,
               "breaks":[
                  {
                     "id":"4591109b-a618-3e0d-e6a0-d42b25b7231f",
                     "notes":{
                        "content":"Lunch break",
                        "contentType":"text"
                     },
                     "start":{
                        "dateTime":"2019-03-18T00:00:00.000Z",
                        "atApprovedLocation":true,
                        "notes":{
                           "content":"Started my break 5 minutes early",
                           "contentType":"text"
                        }
                     },
                     "end":null
                  }
               ]
            }
         }
      }
   ]
}

```
#### <a name="response"></a><span data-ttu-id="b671d-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="b671d-188">Response</span></span>

<span data-ttu-id="b671d-189">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b671d-189">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "responses":[
    {
      "id": "1",
      "status": 200,
      "body":{
        "eTag": "4000ee23-0000-0700-0000-5d1415f60000",
        "error": null
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


