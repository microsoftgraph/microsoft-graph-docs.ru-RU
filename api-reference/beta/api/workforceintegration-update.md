---
title: Обновление рабочей силы
description: Обновление свойств объекта workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6885976681e11640ea3205ce841fe1f6620e626a
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910638"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="da167-103">Обновление рабочей силы</span><span class="sxs-lookup"><span data-stu-id="da167-103">Update workforceintegration</span></span>

<span data-ttu-id="da167-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da167-105">Обновление свойств объекта [workforceintegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="da167-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da167-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da167-106">Permissions</span></span>

<span data-ttu-id="da167-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da167-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da167-109">Permission type</span></span>                        | <span data-ttu-id="da167-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da167-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da167-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da167-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da167-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da167-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="da167-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da167-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da167-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da167-114">Not supported.</span></span> |
| <span data-ttu-id="da167-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da167-115">Application</span></span>                            | <span data-ttu-id="da167-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da167-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da167-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da167-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="da167-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da167-118">Request headers</span></span>

| <span data-ttu-id="da167-119">Имя</span><span class="sxs-lookup"><span data-stu-id="da167-119">Name</span></span>       | <span data-ttu-id="da167-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da167-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da167-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da167-121">Authorization</span></span> | <span data-ttu-id="da167-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="da167-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="da167-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da167-123">Request body</span></span>

<span data-ttu-id="da167-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="da167-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="da167-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="da167-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="da167-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da167-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da167-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="da167-127">Property</span></span>     | <span data-ttu-id="da167-128">Тип</span><span class="sxs-lookup"><span data-stu-id="da167-128">Type</span></span>        | <span data-ttu-id="da167-129">Описание</span><span class="sxs-lookup"><span data-stu-id="da167-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da167-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="da167-130">apiVersion</span></span>|<span data-ttu-id="da167-131">Int32</span><span class="sxs-lookup"><span data-stu-id="da167-131">Int32</span></span>|<span data-ttu-id="da167-132">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="da167-132">API version for the call back url.</span></span> <span data-ttu-id="da167-133">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="da167-133">Start with 1.</span></span>|
|<span data-ttu-id="da167-134">displayName</span><span class="sxs-lookup"><span data-stu-id="da167-134">displayName</span></span>|<span data-ttu-id="da167-135">String</span><span class="sxs-lookup"><span data-stu-id="da167-135">String</span></span>|<span data-ttu-id="da167-136">Имя интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="da167-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="da167-137">шифрование</span><span class="sxs-lookup"><span data-stu-id="da167-137">encryption</span></span>|<span data-ttu-id="da167-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="da167-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="da167-139">Ресурс шифрования интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="da167-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="da167-140">isActive</span><span class="sxs-lookup"><span data-stu-id="da167-140">isActive</span></span>|<span data-ttu-id="da167-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="da167-141">Boolean</span></span>|<span data-ttu-id="da167-142">Указывает, активна ли в настоящее время интеграция с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="da167-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="da167-143">поддерживает</span><span class="sxs-lookup"><span data-stu-id="da167-143">supports</span></span>|<span data-ttu-id="da167-144">string</span><span class="sxs-lookup"><span data-stu-id="da167-144">string</span></span>| <span data-ttu-id="da167-145">Возможные значения: `none` `shift` , , `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="da167-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="da167-146">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="da167-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="da167-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="da167-147">supportedEntities</span></span>|<span data-ttu-id="da167-148">string</span><span class="sxs-lookup"><span data-stu-id="da167-148">string</span></span>| <span data-ttu-id="da167-149">Это свойство заменит **поддержку** в v1.0.</span><span class="sxs-lookup"><span data-stu-id="da167-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="da167-150">Рекомендуется использовать это свойство вместо **поддержки.**</span><span class="sxs-lookup"><span data-stu-id="da167-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="da167-151">Пока **свойство supports** будет поддерживаться в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="da167-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="da167-152">Возможные значения: `none` `shift` , , `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="da167-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="da167-153">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="da167-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="da167-154">url</span><span class="sxs-lookup"><span data-stu-id="da167-154">url</span></span>|<span data-ttu-id="da167-155">String</span><span class="sxs-lookup"><span data-stu-id="da167-155">String</span></span>| <span data-ttu-id="da167-156">URL-адрес интеграции сотрудников для вызовов из службы Shift.</span><span class="sxs-lookup"><span data-stu-id="da167-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="da167-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="da167-157">Response</span></span>

<span data-ttu-id="da167-158">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da167-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da167-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="da167-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="da167-160">Пример 1. Обновление объекта workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="da167-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="da167-161">В следующем примере обновляется **объект workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="da167-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="da167-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="da167-162">Request</span></span>

<span data-ttu-id="da167-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da167-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da167-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="da167-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="da167-165">C#</span><span class="sxs-lookup"><span data-stu-id="da167-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da167-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da167-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da167-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da167-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da167-168">Java</span><span class="sxs-lookup"><span data-stu-id="da167-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da167-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="da167-169">Response</span></span>

<span data-ttu-id="da167-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da167-170">The following is an example of the response.</span></span>

> <span data-ttu-id="da167-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da167-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="da167-173">Пример 2. Создание нового workforceIntegration с включенной фильтрацией на соответствие требованиям SwapRequest</span><span class="sxs-lookup"><span data-stu-id="da167-173">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="da167-174">В следующем примере создается новый **сотрудникIntegration** с включенным фильтром swapRequest.</span><span class="sxs-lookup"><span data-stu-id="da167-174">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="da167-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="da167-175">Request</span></span>

<span data-ttu-id="da167-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da167-176">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="da167-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="da167-177">Response</span></span>

<span data-ttu-id="da167-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da167-178">The following is an example of the response.</span></span>
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
<span data-ttu-id="da167-179">Чтобы создать новую **рабочую** регионацию с включенной фильтрацией правомерности SwapRequest, см. метод [Create.](../api/workforceintegration-post.md)</span><span class="sxs-lookup"><span data-stu-id="da167-179">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="da167-180">Пример 3. Получение подходящих смен, когда SwapRequest включен в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="da167-180">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="da167-181">Взаимодействие между конечными точками интеграции приложения Shifts и сотрудников будет выполняться по существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="da167-181">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="da167-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="da167-182">Request</span></span>

<span data-ttu-id="da167-183">Ниже приводится пример запроса, сделанного shifts на конечную точку интеграции персонала для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="da167-183">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="da167-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="da167-184">Response</span></span>

<span data-ttu-id="da167-185">Ниже приводится пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="da167-185">The following is an example of the response from the workforce integration service.</span></span>
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


