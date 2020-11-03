---
title: Обновление воркфорцеинтегратион
description: Обновление свойств объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e785ca911ce41e0e84060801afae078d867b4a5
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848369"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="c9399-103">Обновление воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="c9399-103">Update workforceintegration</span></span>

<span data-ttu-id="c9399-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9399-105">Обновление свойств объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="c9399-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9399-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9399-106">Permissions</span></span>

<span data-ttu-id="c9399-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9399-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9399-109">Permission type</span></span>                        | <span data-ttu-id="c9399-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9399-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9399-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9399-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9399-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c9399-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="c9399-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9399-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9399-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9399-114">Not supported.</span></span> |
| <span data-ttu-id="c9399-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9399-115">Application</span></span>                            | <span data-ttu-id="c9399-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9399-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9399-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9399-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="c9399-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9399-118">Request headers</span></span>

| <span data-ttu-id="c9399-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c9399-119">Name</span></span>       | <span data-ttu-id="c9399-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9399-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c9399-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9399-121">Authorization</span></span> | <span data-ttu-id="c9399-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c9399-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9399-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9399-123">Request body</span></span>

<span data-ttu-id="c9399-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c9399-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c9399-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c9399-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c9399-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c9399-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9399-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9399-127">Property</span></span>     | <span data-ttu-id="c9399-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c9399-128">Type</span></span>        | <span data-ttu-id="c9399-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c9399-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9399-130">апиверсион</span><span class="sxs-lookup"><span data-stu-id="c9399-130">apiVersion</span></span>|<span data-ttu-id="c9399-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c9399-131">Int32</span></span>|<span data-ttu-id="c9399-132">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="c9399-132">API version for the call back url.</span></span> <span data-ttu-id="c9399-133">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="c9399-133">Start with 1.</span></span>|
|<span data-ttu-id="c9399-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c9399-134">displayName</span></span>|<span data-ttu-id="c9399-135">String</span><span class="sxs-lookup"><span data-stu-id="c9399-135">String</span></span>|<span data-ttu-id="c9399-136">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c9399-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="c9399-137">шифрования</span><span class="sxs-lookup"><span data-stu-id="c9399-137">encryption</span></span>|<span data-ttu-id="c9399-138">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="c9399-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="c9399-139">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="c9399-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="c9399-140">isActive</span><span class="sxs-lookup"><span data-stu-id="c9399-140">isActive</span></span>|<span data-ttu-id="c9399-141">Логический</span><span class="sxs-lookup"><span data-stu-id="c9399-141">Boolean</span></span>|<span data-ttu-id="c9399-142">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="c9399-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="c9399-143">имеется</span><span class="sxs-lookup"><span data-stu-id="c9399-143">supports</span></span>|<span data-ttu-id="c9399-144">string</span><span class="sxs-lookup"><span data-stu-id="c9399-144">string</span></span>| <span data-ttu-id="c9399-145">Возможные значения:,,,, `none` `shift` `swapRequest` `openshift` `openShiftRequest` , `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="c9399-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="c9399-146">Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="c9399-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="c9399-147">суппортедентитиес</span><span class="sxs-lookup"><span data-stu-id="c9399-147">supportedEntities</span></span>|<span data-ttu-id="c9399-148">string</span><span class="sxs-lookup"><span data-stu-id="c9399-148">string</span></span>| <span data-ttu-id="c9399-149">Это свойство **будет заменено** в версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="c9399-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="c9399-150">Мы рекомендуем использовать это свойство вместо **поддерживаемых**.</span><span class="sxs-lookup"><span data-stu-id="c9399-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="c9399-151">Свойство **Supports будет по-** прежнему поддерживаться в бета-версии в течение этого времени.</span><span class="sxs-lookup"><span data-stu-id="c9399-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="c9399-152">Возможные значения:,,,, `none` `shift` `swapRequest` `openshift` `openShiftRequest` , `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="c9399-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="c9399-153">Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="c9399-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="c9399-154">url</span><span class="sxs-lookup"><span data-stu-id="c9399-154">url</span></span>|<span data-ttu-id="c9399-155">String</span><span class="sxs-lookup"><span data-stu-id="c9399-155">String</span></span>| <span data-ttu-id="c9399-156">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="c9399-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="c9399-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9399-157">Response</span></span>

<span data-ttu-id="c9399-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9399-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9399-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9399-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="c9399-160">Пример 1: обновление объекта Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="c9399-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="c9399-161">В приведенном ниже примере показано, как обновить объект **воркфорцеинтегратион** .</span><span class="sxs-lookup"><span data-stu-id="c9399-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="c9399-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9399-162">Request</span></span>

<span data-ttu-id="c9399-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9399-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9399-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9399-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations
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
# <a name="c"></a>[<span data-ttu-id="c9399-165">C#</span><span class="sxs-lookup"><span data-stu-id="c9399-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9399-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9399-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9399-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9399-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9399-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9399-168">Response</span></span>

<span data-ttu-id="c9399-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9399-169">The following is an example of the response.</span></span>

> <span data-ttu-id="c9399-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9399-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="c9399-172">Пример 2: создание нового Воркфорцеинтегратион с включенной функцией Свапрекуест для фильтрации допустимости</span><span class="sxs-lookup"><span data-stu-id="c9399-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="c9399-173">В следующем примере показано, как создать **воркфорцеинтегратион** с свапрекуест, включенным для фильтрации приемлемости.</span><span class="sxs-lookup"><span data-stu-id="c9399-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="c9399-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9399-174">Request</span></span>

<span data-ttu-id="c9399-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9399-175">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="c9399-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9399-176">Response</span></span>

<span data-ttu-id="c9399-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9399-177">The following is an example of the response.</span></span>
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
<span data-ttu-id="c9399-178">Чтобы создать новый **воркфорцеинтегратион** с включенной функцией фильтрации соответствия свапрекуест, ознакомьтесь со статьей метод [CREATE](../api/workforceintegration-post.md) .</span><span class="sxs-lookup"><span data-stu-id="c9399-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="c9399-179">Пример 3: получение подходящих смен при включении Свапрекуест в Елигибилитифилтеринженабледентитиес</span><span class="sxs-lookup"><span data-stu-id="c9399-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="c9399-180">Конечные точки интеграции "взаимодействие между сменами приложения" и "ресурсы" будут соответствовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="c9399-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="c9399-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9399-181">Request</span></span>

<span data-ttu-id="c9399-182">Ниже приведен пример запроса, сделанного сменам конечной точки интеграции сотрудников для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="c9399-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="c9399-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9399-183">Response</span></span>

<span data-ttu-id="c9399-184">Ниже приведен пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="c9399-184">The following is an example of the response from the workforce integration service.</span></span>
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


