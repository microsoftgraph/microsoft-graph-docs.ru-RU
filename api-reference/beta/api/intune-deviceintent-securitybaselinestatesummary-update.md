---
title: Обновление Секуритибаселинестатесуммари
description: Обновление свойств объекта Секуритибаселинестатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5141ce21ce2d0cee08e23a8f12e50c98551bc841
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179455"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="4c77d-103">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="4c77d-103">Update securityBaselineStateSummary</span></span>

> <span data-ttu-id="4c77d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c77d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c77d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c77d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c77d-106">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4c77d-106">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c77d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c77d-107">Prerequisites</span></span>
<span data-ttu-id="4c77d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c77d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c77d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c77d-110">Permission type</span></span>|<span data-ttu-id="4c77d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c77d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c77d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c77d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c77d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c77d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c77d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c77d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c77d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c77d-115">Not supported.</span></span>|
|<span data-ttu-id="4c77d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c77d-116">Application</span></span>|<span data-ttu-id="4c77d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c77d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c77d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c77d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4c77d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c77d-119">Request headers</span></span>
|<span data-ttu-id="4c77d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c77d-120">Header</span></span>|<span data-ttu-id="4c77d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c77d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c77d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c77d-122">Authorization</span></span>|<span data-ttu-id="4c77d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c77d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c77d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4c77d-124">Accept</span></span>|<span data-ttu-id="4c77d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c77d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c77d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c77d-126">Request body</span></span>
<span data-ttu-id="4c77d-127">В тексте запроса добавьте представление объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c77d-127">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="4c77d-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4c77d-128">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="4c77d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c77d-129">Property</span></span>|<span data-ttu-id="4c77d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c77d-130">Type</span></span>|<span data-ttu-id="4c77d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c77d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c77d-132">id</span><span class="sxs-lookup"><span data-stu-id="4c77d-132">id</span></span>|<span data-ttu-id="4c77d-133">String</span><span class="sxs-lookup"><span data-stu-id="4c77d-133">String</span></span>|<span data-ttu-id="4c77d-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="4c77d-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4c77d-135">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="4c77d-135">secureCount</span></span>|<span data-ttu-id="4c77d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-136">Int32</span></span>|<span data-ttu-id="4c77d-137">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="4c77d-137">Number of secure devices</span></span>|
|<span data-ttu-id="4c77d-138">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="4c77d-138">notSecureCount</span></span>|<span data-ttu-id="4c77d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-139">Int32</span></span>|<span data-ttu-id="4c77d-140">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="4c77d-140">Number of not secure devices</span></span>|
|<span data-ttu-id="4c77d-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4c77d-141">unknownCount</span></span>|<span data-ttu-id="4c77d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-142">Int32</span></span>|<span data-ttu-id="4c77d-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="4c77d-143">Number of unknown devices</span></span>|
|<span data-ttu-id="4c77d-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4c77d-144">errorCount</span></span>|<span data-ttu-id="4c77d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-145">Int32</span></span>|<span data-ttu-id="4c77d-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4c77d-146">Number of error devices</span></span>|
|<span data-ttu-id="4c77d-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4c77d-147">conflictCount</span></span>|<span data-ttu-id="4c77d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-148">Int32</span></span>|<span data-ttu-id="4c77d-149">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="4c77d-149">Number of conflict devices</span></span>|
|<span data-ttu-id="4c77d-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4c77d-150">notApplicableCount</span></span>|<span data-ttu-id="4c77d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4c77d-151">Int32</span></span>|<span data-ttu-id="4c77d-152">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4c77d-152">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="4c77d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c77d-153">Response</span></span>
<span data-ttu-id="4c77d-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c77d-154">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c77d-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4c77d-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c77d-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c77d-156">Request</span></span>
<span data-ttu-id="4c77d-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c77d-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="4c77d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c77d-158">Response</span></span>
<span data-ttu-id="4c77d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c77d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```




