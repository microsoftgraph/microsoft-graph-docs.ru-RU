---
title: Обновление Воркфорцеинтегратион
description: Обновление свойств объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ff45c62726c5efc986593e3e949ffacdb115a15
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849083"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="6308c-103">Обновление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="6308c-103">Update workforceIntegration</span></span>

<span data-ttu-id="6308c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6308c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6308c-105">Обновление свойств объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="6308c-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6308c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6308c-106">Permissions</span></span>

<span data-ttu-id="6308c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6308c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6308c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6308c-109">Permission type</span></span>                        | <span data-ttu-id="6308c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6308c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6308c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6308c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6308c-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6308c-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="6308c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6308c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6308c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6308c-114">Not supported.</span></span> |
| <span data-ttu-id="6308c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6308c-115">Application</span></span>                            | <span data-ttu-id="6308c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6308c-116">Not supported.</span></span> |

> <span data-ttu-id="6308c-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6308c-117">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="6308c-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="6308c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6308c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6308c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="6308c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6308c-120">Request headers</span></span>

| <span data-ttu-id="6308c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6308c-121">Name</span></span>       | <span data-ttu-id="6308c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6308c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6308c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6308c-123">Authorization</span></span> | <span data-ttu-id="6308c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6308c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6308c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6308c-125">Request body</span></span>

<span data-ttu-id="6308c-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6308c-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6308c-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6308c-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6308c-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6308c-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6308c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6308c-129">Property</span></span>     | <span data-ttu-id="6308c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6308c-130">Type</span></span>        | <span data-ttu-id="6308c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6308c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6308c-132">апиверсион</span><span class="sxs-lookup"><span data-stu-id="6308c-132">apiVersion</span></span>|<span data-ttu-id="6308c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6308c-133">Int32</span></span>|<span data-ttu-id="6308c-134">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="6308c-134">API version for the call back URL.</span></span> <span data-ttu-id="6308c-135">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="6308c-135">Start with 1.</span></span>|
|<span data-ttu-id="6308c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6308c-136">displayName</span></span>|<span data-ttu-id="6308c-137">String</span><span class="sxs-lookup"><span data-stu-id="6308c-137">String</span></span>|<span data-ttu-id="6308c-138">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6308c-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="6308c-139">шифрования</span><span class="sxs-lookup"><span data-stu-id="6308c-139">encryption</span></span>|<span data-ttu-id="6308c-140">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="6308c-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="6308c-141">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="6308c-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="6308c-142">isActive</span><span class="sxs-lookup"><span data-stu-id="6308c-142">isActive</span></span>|<span data-ttu-id="6308c-143">Логический</span><span class="sxs-lookup"><span data-stu-id="6308c-143">Boolean</span></span>|<span data-ttu-id="6308c-144">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="6308c-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="6308c-145">суппортедентитиес</span><span class="sxs-lookup"><span data-stu-id="6308c-145">supportedEntities</span></span>|<span data-ttu-id="6308c-146">string</span><span class="sxs-lookup"><span data-stu-id="6308c-146">string</span></span>| <span data-ttu-id="6308c-147">Возможные значения: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="6308c-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="6308c-148">Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="6308c-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="6308c-149">url</span><span class="sxs-lookup"><span data-stu-id="6308c-149">url</span></span>|<span data-ttu-id="6308c-150">String</span><span class="sxs-lookup"><span data-stu-id="6308c-150">String</span></span>| <span data-ttu-id="6308c-151">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="6308c-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="6308c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6308c-152">Response</span></span>

<span data-ttu-id="6308c-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6308c-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6308c-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="6308c-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6308c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6308c-155">Request</span></span>

<span data-ttu-id="6308c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6308c-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6308c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6308c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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
  "supportedEntities": "supportedEntities-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6308c-158">C#</span><span class="sxs-lookup"><span data-stu-id="6308c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6308c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6308c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6308c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6308c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6308c-161">Java</span><span class="sxs-lookup"><span data-stu-id="6308c-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6308c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6308c-162">Response</span></span>

<span data-ttu-id="6308c-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6308c-163">The following is an example of the response.</span></span>

> <span data-ttu-id="6308c-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6308c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="6308c-166">Примеры использования сущностей Воркфорцеинтегратион для фильтрации по допустимости правил WFM</span><span class="sxs-lookup"><span data-stu-id="6308c-166">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="6308c-167">Вариант использования: замена существующего Воркфорцеинтегратион для включения Свапрекуест для фильтрации допустимости</span><span class="sxs-lookup"><span data-stu-id="6308c-167">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="6308c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6308c-168">Request</span></span>

<span data-ttu-id="6308c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6308c-169">The following is an example of the request.</span></span> 
```
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationid}
{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    - "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
```
### <a name="response"></a><span data-ttu-id="6308c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="6308c-170">Response</span></span>

<span data-ttu-id="6308c-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6308c-171">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
Content-type: application/json
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
<span data-ttu-id="6308c-172">Чтобы узнать, как создать новый воркфорцеинтегратион с включенной функцией фильтрации соответствия Свапрекуест, ознакомьтесь со статьей [Create (создать](../api/workforceintegration-post.md)).</span><span class="sxs-lookup"><span data-stu-id="6308c-172">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="6308c-173">Пример извлечения подходящих смен при включении Свапрекуест в Елигибилитифилтеринженабледентитиес</span><span class="sxs-lookup"><span data-stu-id="6308c-173">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="6308c-174">Конечные точки интеграции "взаимодействие между сменами приложения" и "ресурсы" будут соответствовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="6308c-174">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="6308c-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="6308c-175">Request</span></span>

<span data-ttu-id="6308c-176">Ниже приведен пример запроса, сделанного сменам конечной точки интеграции сотрудников для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="6308c-176">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="6308c-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="6308c-177">Response</span></span>

<span data-ttu-id="6308c-178">Ниже приведен пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="6308c-178">The following is an example of the response from the workforce integration service.</span></span>
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

