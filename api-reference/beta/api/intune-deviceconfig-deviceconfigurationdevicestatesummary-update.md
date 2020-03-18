---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 171202d55659cab7b1c01ee793b14e34f6dcb64d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42754099"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="ae152-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ae152-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="ae152-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae152-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae152-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae152-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae152-106">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ae152-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae152-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ae152-107">Prerequisites</span></span>
<span data-ttu-id="ae152-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae152-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae152-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae152-110">Permission type</span></span>|<span data-ttu-id="ae152-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae152-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae152-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae152-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae152-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae152-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae152-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae152-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae152-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae152-115">Not supported.</span></span>|
|<span data-ttu-id="ae152-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae152-116">Application</span></span>|<span data-ttu-id="ae152-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae152-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae152-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae152-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ae152-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae152-119">Request headers</span></span>
|<span data-ttu-id="ae152-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae152-120">Header</span></span>|<span data-ttu-id="ae152-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ae152-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae152-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae152-122">Authorization</span></span>|<span data-ttu-id="ae152-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae152-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae152-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ae152-124">Accept</span></span>|<span data-ttu-id="ae152-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae152-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae152-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae152-126">Request body</span></span>
<span data-ttu-id="ae152-127">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae152-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="ae152-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ae152-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="ae152-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae152-129">Property</span></span>|<span data-ttu-id="ae152-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ae152-130">Type</span></span>|<span data-ttu-id="ae152-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ae152-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae152-132">id</span><span class="sxs-lookup"><span data-stu-id="ae152-132">id</span></span>|<span data-ttu-id="ae152-133">String</span><span class="sxs-lookup"><span data-stu-id="ae152-133">String</span></span>|<span data-ttu-id="ae152-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae152-134">Key of the entity.</span></span>|
|<span data-ttu-id="ae152-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-135">unknownDeviceCount</span></span>|<span data-ttu-id="ae152-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-136">Int32</span></span>|<span data-ttu-id="ae152-137">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="ae152-137">Number of unknown devices</span></span>|
|<span data-ttu-id="ae152-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="ae152-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-139">Int32</span></span>|<span data-ttu-id="ae152-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="ae152-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="ae152-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-141">compliantDeviceCount</span></span>|<span data-ttu-id="ae152-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-142">Int32</span></span>|<span data-ttu-id="ae152-143">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ae152-143">Number of compliant devices</span></span>|
|<span data-ttu-id="ae152-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-144">remediatedDeviceCount</span></span>|<span data-ttu-id="ae152-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-145">Int32</span></span>|<span data-ttu-id="ae152-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="ae152-146">Number of remediated devices</span></span>|
|<span data-ttu-id="ae152-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ae152-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-148">Int32</span></span>|<span data-ttu-id="ae152-149">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ae152-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ae152-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-150">errorDeviceCount</span></span>|<span data-ttu-id="ae152-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-151">Int32</span></span>|<span data-ttu-id="ae152-152">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="ae152-152">Number of error devices</span></span>|
|<span data-ttu-id="ae152-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae152-153">conflictDeviceCount</span></span>|<span data-ttu-id="ae152-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ae152-154">Int32</span></span>|<span data-ttu-id="ae152-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="ae152-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ae152-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae152-156">Response</span></span>
<span data-ttu-id="ae152-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae152-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae152-158">Пример</span><span class="sxs-lookup"><span data-stu-id="ae152-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae152-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae152-159">Request</span></span>
<span data-ttu-id="ae152-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae152-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="ae152-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae152-161">Response</span></span>
<span data-ttu-id="ae152-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae152-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




