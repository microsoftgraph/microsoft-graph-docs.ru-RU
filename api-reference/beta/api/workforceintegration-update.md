---
title: Обновление реинтеграции рабочей силы
description: Обновление свойств объекта по реинтеграции рабочей силы.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2da287f8b78beae39ce5842307c08ff15ef78007
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054681"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="dfef9-103">Обновление реинтеграции рабочей силы</span><span class="sxs-lookup"><span data-stu-id="dfef9-103">Update workforceintegration</span></span>

<span data-ttu-id="dfef9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfef9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfef9-105">Обновление свойств объекта [по реинтеграции](../resources/workforceintegration.md) рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="dfef9-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfef9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfef9-106">Permissions</span></span>

<span data-ttu-id="dfef9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfef9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfef9-109">Permission type</span></span>                        | <span data-ttu-id="dfef9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfef9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfef9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfef9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfef9-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfef9-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="dfef9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfef9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfef9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfef9-114">Not supported.</span></span> |
| <span data-ttu-id="dfef9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfef9-115">Application</span></span>                            | <span data-ttu-id="dfef9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfef9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfef9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfef9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="dfef9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfef9-118">Request headers</span></span>

| <span data-ttu-id="dfef9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dfef9-119">Name</span></span>       | <span data-ttu-id="dfef9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dfef9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dfef9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfef9-121">Authorization</span></span> | <span data-ttu-id="dfef9-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="dfef9-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfef9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfef9-123">Request body</span></span>

<span data-ttu-id="dfef9-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dfef9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dfef9-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dfef9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dfef9-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dfef9-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dfef9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfef9-127">Property</span></span>     | <span data-ttu-id="dfef9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dfef9-128">Type</span></span>        | <span data-ttu-id="dfef9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dfef9-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfef9-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="dfef9-130">apiVersion</span></span>|<span data-ttu-id="dfef9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="dfef9-131">Int32</span></span>|<span data-ttu-id="dfef9-132">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="dfef9-132">API version for the call back url.</span></span> <span data-ttu-id="dfef9-133">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="dfef9-133">Start with 1.</span></span>|
|<span data-ttu-id="dfef9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="dfef9-134">displayName</span></span>|<span data-ttu-id="dfef9-135">String</span><span class="sxs-lookup"><span data-stu-id="dfef9-135">String</span></span>|<span data-ttu-id="dfef9-136">Имя интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="dfef9-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="dfef9-137">шифрование</span><span class="sxs-lookup"><span data-stu-id="dfef9-137">encryption</span></span>|<span data-ttu-id="dfef9-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="dfef9-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="dfef9-139">Ресурс шифрования интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="dfef9-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="dfef9-140">isActive</span><span class="sxs-lookup"><span data-stu-id="dfef9-140">isActive</span></span>|<span data-ttu-id="dfef9-141">Логический</span><span class="sxs-lookup"><span data-stu-id="dfef9-141">Boolean</span></span>|<span data-ttu-id="dfef9-142">Указывает, является ли эта интеграция рабочей силы активной и доступной в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="dfef9-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="dfef9-143">поддерживает</span><span class="sxs-lookup"><span data-stu-id="dfef9-143">supports</span></span>|<span data-ttu-id="dfef9-144">String</span><span class="sxs-lookup"><span data-stu-id="dfef9-144">string</span></span>| <span data-ttu-id="dfef9-145">Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="dfef9-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="dfef9-146">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.</span><span class="sxs-lookup"><span data-stu-id="dfef9-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="dfef9-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="dfef9-147">supportedEntities</span></span>|<span data-ttu-id="dfef9-148">String</span><span class="sxs-lookup"><span data-stu-id="dfef9-148">string</span></span>| <span data-ttu-id="dfef9-149">Это свойство заменит **поддержки** в v1.0.</span><span class="sxs-lookup"><span data-stu-id="dfef9-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="dfef9-150">Рекомендуется использовать это свойство вместо **поддержки.**</span><span class="sxs-lookup"><span data-stu-id="dfef9-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="dfef9-151">Свойство **поддерживается** в бета-версии в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="dfef9-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="dfef9-152">Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="dfef9-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="dfef9-153">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.</span><span class="sxs-lookup"><span data-stu-id="dfef9-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="dfef9-154">url</span><span class="sxs-lookup"><span data-stu-id="dfef9-154">url</span></span>|<span data-ttu-id="dfef9-155">String</span><span class="sxs-lookup"><span data-stu-id="dfef9-155">String</span></span>| <span data-ttu-id="dfef9-156">URL-адрес интеграции рабочей силы для вызовов из службы Shift.</span><span class="sxs-lookup"><span data-stu-id="dfef9-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="dfef9-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfef9-157">Response</span></span>

<span data-ttu-id="dfef9-158">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dfef9-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfef9-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="dfef9-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="dfef9-160">Пример 1. Обновление объекта workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="dfef9-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="dfef9-161">В следующем примере обновляется **объект workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="dfef9-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="dfef9-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfef9-162">Request</span></span>

<span data-ttu-id="dfef9-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfef9-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfef9-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfef9-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dfef9-165">C#</span><span class="sxs-lookup"><span data-stu-id="dfef9-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfef9-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfef9-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfef9-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfef9-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfef9-168">Java</span><span class="sxs-lookup"><span data-stu-id="dfef9-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfef9-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfef9-169">Response</span></span>

<span data-ttu-id="dfef9-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dfef9-170">The following is an example of the response.</span></span>

> <span data-ttu-id="dfef9-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfef9-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="dfef9-172">Пример 2. Создание новой рабочей силыИнтеграция с помощью SwapRequest, включенной для фильтрации прав</span><span class="sxs-lookup"><span data-stu-id="dfef9-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="dfef9-173">В следующем примере создается новая **рабочая силаИнтеграция** с поддержкой SwapRequest для фильтрации прав.</span><span class="sxs-lookup"><span data-stu-id="dfef9-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="dfef9-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfef9-174">Request</span></span>

<span data-ttu-id="dfef9-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfef9-175">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="dfef9-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfef9-176">Response</span></span>

<span data-ttu-id="dfef9-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dfef9-177">The following is an example of the response.</span></span>
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
<span data-ttu-id="dfef9-178">Чтобы создать новую **рабочую силуИнтеграция** с помощью SwapRequest, включенной для фильтрации прав, см. в [методе Create.](../api/workforceintegration-post.md)</span><span class="sxs-lookup"><span data-stu-id="dfef9-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="dfef9-179">Пример 3. Получение подходящих сдвигов при включении SwapRequest в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="dfef9-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="dfef9-180">Взаимодействие между конечными точками интеграции shifts и рабочей силой будет следовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="dfef9-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="dfef9-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfef9-181">Request</span></span>

<span data-ttu-id="dfef9-182">Ниже приводится пример запроса shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span><span class="sxs-lookup"><span data-stu-id="dfef9-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="dfef9-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfef9-183">Response</span></span>

<span data-ttu-id="dfef9-184">Ниже приводится пример ответа службы интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="dfef9-184">The following is an example of the response from the workforce integration service.</span></span>
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
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


