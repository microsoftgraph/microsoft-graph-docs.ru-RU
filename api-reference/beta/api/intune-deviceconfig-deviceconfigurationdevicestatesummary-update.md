---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6afdd4559e21453dc615f4adfd736b98977746d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449168"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="f7f05-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f7f05-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="f7f05-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f7f05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7f05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7f05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7f05-107">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7f05-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7f05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7f05-108">Prerequisites</span></span>
<span data-ttu-id="f7f05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7f05-111">Permission type</span></span>|<span data-ttu-id="f7f05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7f05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7f05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7f05-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f05-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7f05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7f05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f05-116">Not supported.</span></span>|
|<span data-ttu-id="f7f05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7f05-117">Application</span></span>|<span data-ttu-id="f7f05-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f05-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7f05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f7f05-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7f05-120">Request headers</span></span>
|<span data-ttu-id="f7f05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7f05-121">Header</span></span>|<span data-ttu-id="f7f05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7f05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7f05-123">Authorization</span></span>|<span data-ttu-id="f7f05-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7f05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7f05-125">Accept</span></span>|<span data-ttu-id="f7f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7f05-127">Request body</span></span>
<span data-ttu-id="f7f05-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7f05-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="f7f05-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7f05-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="f7f05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7f05-130">Property</span></span>|<span data-ttu-id="f7f05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7f05-131">Type</span></span>|<span data-ttu-id="f7f05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f05-133">id</span><span class="sxs-lookup"><span data-stu-id="f7f05-133">id</span></span>|<span data-ttu-id="f7f05-134">String</span><span class="sxs-lookup"><span data-stu-id="f7f05-134">String</span></span>|<span data-ttu-id="f7f05-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7f05-135">Key of the entity.</span></span>|
|<span data-ttu-id="f7f05-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-136">unknownDeviceCount</span></span>|<span data-ttu-id="f7f05-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-137">Int32</span></span>|<span data-ttu-id="f7f05-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="f7f05-138">Number of unknown devices</span></span>|
|<span data-ttu-id="f7f05-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="f7f05-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-140">Int32</span></span>|<span data-ttu-id="f7f05-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f7f05-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="f7f05-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-142">compliantDeviceCount</span></span>|<span data-ttu-id="f7f05-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-143">Int32</span></span>|<span data-ttu-id="f7f05-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f7f05-144">Number of compliant devices</span></span>|
|<span data-ttu-id="f7f05-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-145">remediatedDeviceCount</span></span>|<span data-ttu-id="f7f05-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-146">Int32</span></span>|<span data-ttu-id="f7f05-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f7f05-147">Number of remediated devices</span></span>|
|<span data-ttu-id="f7f05-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f7f05-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-149">Int32</span></span>|<span data-ttu-id="f7f05-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f7f05-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f7f05-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-151">errorDeviceCount</span></span>|<span data-ttu-id="f7f05-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-152">Int32</span></span>|<span data-ttu-id="f7f05-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f7f05-153">Number of error devices</span></span>|
|<span data-ttu-id="f7f05-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7f05-154">conflictDeviceCount</span></span>|<span data-ttu-id="f7f05-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f05-155">Int32</span></span>|<span data-ttu-id="f7f05-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="f7f05-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f7f05-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f05-157">Response</span></span>
<span data-ttu-id="f7f05-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7f05-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7f05-159">Пример</span><span class="sxs-lookup"><span data-stu-id="f7f05-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7f05-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7f05-160">Request</span></span>
<span data-ttu-id="f7f05-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7f05-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7f05-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f05-162">Response</span></span>
<span data-ttu-id="f7f05-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7f05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





