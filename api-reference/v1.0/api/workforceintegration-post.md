---
title: Создание Воркфорцеинтегратион
description: Создание нового объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 74481ea9bcb843b89bb1de3fdf444e359762aaa4
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154040"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="68173-103">Создание Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="68173-103">Create workforceIntegration</span></span>

<span data-ttu-id="68173-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68173-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68173-105">Создание нового объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="68173-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>
<span data-ttu-id="68173-106">Вы можете настроить, какие сущности вы хотите получать при синхронных уведомлениях об изменениях и настройке сущностей для настройки фильтрации с помощью правил WFM, в том числе запросов на замену.</span><span class="sxs-lookup"><span data-stu-id="68173-106">You can set up which entities you want to receive Shifts synchronous change notifications on and set entities to configure filtering by WFM rules eligibility for, including swap requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="68173-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68173-107">Permissions</span></span>

<span data-ttu-id="68173-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68173-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68173-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68173-110">Permission type</span></span>                        | <span data-ttu-id="68173-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68173-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68173-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68173-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="68173-113">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="68173-113">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="68173-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68173-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68173-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68173-115">Not supported.</span></span> |
| <span data-ttu-id="68173-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68173-116">Application</span></span>                            | <span data-ttu-id="68173-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68173-117">Not supported.</span></span> |

> <span data-ttu-id="68173-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="68173-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="68173-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="68173-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="68173-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68173-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="68173-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68173-121">Request headers</span></span>

| <span data-ttu-id="68173-122">Имя</span><span class="sxs-lookup"><span data-stu-id="68173-122">Name</span></span>          | <span data-ttu-id="68173-123">Описание</span><span class="sxs-lookup"><span data-stu-id="68173-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68173-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68173-124">Authorization</span></span> | <span data-ttu-id="68173-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68173-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68173-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68173-127">Content-type</span></span> | <span data-ttu-id="68173-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68173-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68173-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68173-130">Request body</span></span>

<span data-ttu-id="68173-131">В тексте запроса добавьте представление объекта [воркфорцеинтегратион](../resources/workforceintegration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68173-131">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68173-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="68173-132">Response</span></span>

<span data-ttu-id="68173-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68173-133">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68173-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="68173-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68173-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="68173-135">Request</span></span>

<span data-ttu-id="68173-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68173-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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
---


### <a name="response"></a><span data-ttu-id="68173-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="68173-137">Response</span></span>

<span data-ttu-id="68173-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68173-138">The following is an example of the response.</span></span>

> <span data-ttu-id="68173-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68173-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-for-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="68173-141">Примеры для вариантов использования объекта Воркфорцеинтегратион для фильтрации по допустимости правил WFM</span><span class="sxs-lookup"><span data-stu-id="68173-141">Examples for Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="68173-142">Вариант использования: создание нового Воркфорцеинтегратион с включенной функцией Свапрекуест для фильтрации допустимости</span><span class="sxs-lookup"><span data-stu-id="68173-142">Use case: Create a new WorkforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="68173-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="68173-143">Request</span></span>

<span data-ttu-id="68173-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68173-144">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/
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
Authorization: Bearer {token}
Content-type: application/json
```
### <a name="response"></a><span data-ttu-id="68173-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="68173-145">Response</span></span>

<span data-ttu-id="68173-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68173-146">The following is an example of the response.</span></span>
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
<span data-ttu-id="68173-147">Чтобы узнать, как обновить существующую воркфорцеинтегратион с Свапрекуест, включенной для фильтрации допустимости, ознакомьтесь со статьей [Update](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="68173-147">To see how to update an existing workforceintegration with SwapRequest enabled for eligibility filtering, see [Update](../api/workforceintegration-update.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="68173-148">Пример извлечения подходящих смен при включении Свапрекуест в Елигибилитифилтеринженабледентитиес</span><span class="sxs-lookup"><span data-stu-id="68173-148">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="68173-149">Конечные точки интеграции "взаимодействие между сменами приложения" и "ресурсы" будут соответствовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="68173-149">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="68173-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="68173-150">Request</span></span>

<span data-ttu-id="68173-151">Ниже приведен пример запроса, сделанного сменам конечной точки интеграции сотрудников для получения подходящих смен для запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="68173-151">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="68173-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="68173-152">Response</span></span>

<span data-ttu-id="68173-153">Ниже приведен пример ответа от службы интеграции сотрудников.</span><span class="sxs-lookup"><span data-stu-id="68173-153">The following is an example of the response from the workforce integration service.</span></span>
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
