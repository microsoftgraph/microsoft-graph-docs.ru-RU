---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: add8609cf9ce7a8f791e350626a3accee8d74b5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017527"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="9dfdf-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9dfdf-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="9dfdf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dfdf-105">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9dfdf-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dfdf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9dfdf-106">Prerequisites</span></span>
<span data-ttu-id="9dfdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dfdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfdf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dfdf-109">Permission type</span></span>|<span data-ttu-id="9dfdf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dfdf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dfdf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dfdf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9dfdf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dfdf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9dfdf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dfdf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dfdf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-114">Not supported.</span></span>|
|<span data-ttu-id="9dfdf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dfdf-115">Application</span></span>|<span data-ttu-id="9dfdf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dfdf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dfdf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9dfdf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dfdf-118">Request headers</span></span>
|<span data-ttu-id="9dfdf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dfdf-119">Header</span></span>|<span data-ttu-id="9dfdf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9dfdf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dfdf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dfdf-121">Authorization</span></span>|<span data-ttu-id="9dfdf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dfdf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9dfdf-123">Accept</span></span>|<span data-ttu-id="9dfdf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9dfdf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dfdf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9dfdf-125">Request body</span></span>
<span data-ttu-id="9dfdf-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="9dfdf-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9dfdf-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="9dfdf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dfdf-128">Property</span></span>|<span data-ttu-id="9dfdf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9dfdf-129">Type</span></span>|<span data-ttu-id="9dfdf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9dfdf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dfdf-131">id</span><span class="sxs-lookup"><span data-stu-id="9dfdf-131">id</span></span>|<span data-ttu-id="9dfdf-132">String</span><span class="sxs-lookup"><span data-stu-id="9dfdf-132">String</span></span>|<span data-ttu-id="9dfdf-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-133">Key of the entity.</span></span>|
|<span data-ttu-id="9dfdf-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-134">unknownDeviceCount</span></span>|<span data-ttu-id="9dfdf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-135">Int32</span></span>|<span data-ttu-id="9dfdf-136">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-136">Number of unknown devices</span></span>|
|<span data-ttu-id="9dfdf-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="9dfdf-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-138">Int32</span></span>|<span data-ttu-id="9dfdf-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="9dfdf-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-140">compliantDeviceCount</span></span>|<span data-ttu-id="9dfdf-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-141">Int32</span></span>|<span data-ttu-id="9dfdf-142">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-142">Number of compliant devices</span></span>|
|<span data-ttu-id="9dfdf-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-143">remediatedDeviceCount</span></span>|<span data-ttu-id="9dfdf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-144">Int32</span></span>|<span data-ttu-id="9dfdf-145">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-145">Number of remediated devices</span></span>|
|<span data-ttu-id="9dfdf-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9dfdf-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-147">Int32</span></span>|<span data-ttu-id="9dfdf-148">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="9dfdf-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-149">errorDeviceCount</span></span>|<span data-ttu-id="9dfdf-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-150">Int32</span></span>|<span data-ttu-id="9dfdf-151">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-151">Number of error devices</span></span>|
|<span data-ttu-id="9dfdf-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9dfdf-152">conflictDeviceCount</span></span>|<span data-ttu-id="9dfdf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9dfdf-153">Int32</span></span>|<span data-ttu-id="9dfdf-154">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="9dfdf-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdf-155">Response</span></span>
<span data-ttu-id="9dfdf-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dfdf-157">Пример</span><span class="sxs-lookup"><span data-stu-id="9dfdf-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dfdf-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dfdf-158">Request</span></span>
<span data-ttu-id="9dfdf-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="9dfdf-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfdf-160">Response</span></span>
<span data-ttu-id="9dfdf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dfdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



