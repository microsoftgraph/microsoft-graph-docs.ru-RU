---
title: Обновление workforceIntegration
description: Обновление свойств объекта workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97a902f38b983105a1815250071b3ef7f8b3d7bd
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910529"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="3485d-103">Обновление workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="3485d-103">Update workforceIntegration</span></span>

<span data-ttu-id="3485d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3485d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3485d-105">Обновление свойств объекта [workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="3485d-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3485d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3485d-106">Permissions</span></span>

<span data-ttu-id="3485d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3485d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3485d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3485d-109">Permission type</span></span>                        | <span data-ttu-id="3485d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3485d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3485d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3485d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3485d-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3485d-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="3485d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3485d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3485d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3485d-114">Not supported.</span></span> |
| <span data-ttu-id="3485d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3485d-115">Application</span></span>                            | <span data-ttu-id="3485d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3485d-116">Not supported.</span></span> |

> <span data-ttu-id="3485d-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3485d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3485d-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="3485d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3485d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3485d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="3485d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3485d-120">Request headers</span></span>

| <span data-ttu-id="3485d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3485d-121">Name</span></span>       | <span data-ttu-id="3485d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3485d-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3485d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3485d-123">Authorization</span></span> | <span data-ttu-id="3485d-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3485d-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3485d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3485d-125">Request body</span></span>

<span data-ttu-id="3485d-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3485d-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3485d-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3485d-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3485d-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3485d-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3485d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3485d-129">Property</span></span>     | <span data-ttu-id="3485d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3485d-130">Type</span></span>        | <span data-ttu-id="3485d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3485d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3485d-132">apiVersion</span><span class="sxs-lookup"><span data-stu-id="3485d-132">apiVersion</span></span>|<span data-ttu-id="3485d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3485d-133">Int32</span></span>|<span data-ttu-id="3485d-134">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="3485d-134">API version for the call back URL.</span></span> <span data-ttu-id="3485d-135">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="3485d-135">Start with 1.</span></span>|
|<span data-ttu-id="3485d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3485d-136">displayName</span></span>|<span data-ttu-id="3485d-137">String</span><span class="sxs-lookup"><span data-stu-id="3485d-137">String</span></span>|<span data-ttu-id="3485d-138">Имя интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="3485d-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="3485d-139">шифрование</span><span class="sxs-lookup"><span data-stu-id="3485d-139">encryption</span></span>|<span data-ttu-id="3485d-140">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="3485d-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="3485d-141">Ресурс шифрования интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="3485d-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="3485d-142">isActive</span><span class="sxs-lookup"><span data-stu-id="3485d-142">isActive</span></span>|<span data-ttu-id="3485d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="3485d-143">Boolean</span></span>|<span data-ttu-id="3485d-144">Указывает, активна ли в настоящее время интеграция с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="3485d-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="3485d-145">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="3485d-145">supportedEntities</span></span>|<span data-ttu-id="3485d-146">string</span><span class="sxs-lookup"><span data-stu-id="3485d-146">string</span></span>| <span data-ttu-id="3485d-147">Возможные значения: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="3485d-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="3485d-148">Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="3485d-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="3485d-149">url</span><span class="sxs-lookup"><span data-stu-id="3485d-149">url</span></span>|<span data-ttu-id="3485d-150">String</span><span class="sxs-lookup"><span data-stu-id="3485d-150">String</span></span>| <span data-ttu-id="3485d-151">URL-адрес интеграции сотрудников для службы переключе вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="3485d-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="3485d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3485d-152">Response</span></span>

<span data-ttu-id="3485d-153">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3485d-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3485d-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="3485d-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3485d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3485d-155">Request</span></span>

<span data-ttu-id="3485d-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3485d-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3485d-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="3485d-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
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
# <a name="c"></a>[<span data-ttu-id="3485d-158">C#</span><span class="sxs-lookup"><span data-stu-id="3485d-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3485d-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3485d-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3485d-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3485d-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3485d-161">Java</span><span class="sxs-lookup"><span data-stu-id="3485d-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="3485d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3485d-162">Response</span></span>

<span data-ttu-id="3485d-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3485d-163">The following is an example of the response.</span></span>

> <span data-ttu-id="3485d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3485d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="3485d-166">Примеры использования объекта WorkforceIntegration для фильтрации по правилам WFM</span><span class="sxs-lookup"><span data-stu-id="3485d-166">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="3485d-167">Пример использования: замените существующий WorkforceIntegration, чтобы включить SwapRequest для фильтрации правомерности</span><span class="sxs-lookup"><span data-stu-id="3485d-167">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="3485d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="3485d-168">Request</span></span>

<span data-ttu-id="3485d-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3485d-169">The following is an example of the request.</span></span> 
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
### <a name="response"></a><span data-ttu-id="3485d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3485d-170">Response</span></span>

<span data-ttu-id="3485d-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3485d-171">The following is an example of the response.</span></span>
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
<span data-ttu-id="3485d-172">Чтобы узнать, как создать новую рабочую силу с помощью SwapRequest, включенной для фильтрации правомерности, см. [создание](../api/workforceintegration-post.md).</span><span class="sxs-lookup"><span data-stu-id="3485d-172">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="3485d-173">Пример получения подходящих смен, когда SwapRequest включен в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="3485d-173">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="3485d-174">Взаимодействие между конечными точками интеграции приложения Shifts и сотрудников будет выполняться по существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="3485d-174">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="3485d-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="3485d-175">Request</span></span>

<span data-ttu-id="3485d-176">Ниже приводится пример запроса, сделанного shifts на конечную точку интеграции персонала для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="3485d-176">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="3485d-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="3485d-177">Response</span></span>

<span data-ttu-id="3485d-178">Ниже приводится пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="3485d-178">The following is an example of the response from the workforce integration service.</span></span>
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

