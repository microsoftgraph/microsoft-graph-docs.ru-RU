---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53233df580805b69970573f41a6071b44c3231c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758332"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="1d3d8-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d3d8-103">Create iosUpdateConfiguration</span></span>

<span data-ttu-id="1d3d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d3d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d3d8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d3d8-106">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d3d8-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1d3d8-107">Prerequisites</span></span>
<span data-ttu-id="1d3d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d3d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d3d8-110">Permission type</span></span>|<span data-ttu-id="1d3d8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d3d8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d3d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d3d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d3d8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3d8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d3d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d3d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d3d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-115">Not supported.</span></span>|
|<span data-ttu-id="1d3d8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1d3d8-116">Application</span></span>|<span data-ttu-id="1d3d8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3d8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d3d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d3d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d3d8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d3d8-119">Request headers</span></span>
|<span data-ttu-id="1d3d8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d3d8-120">Header</span></span>|<span data-ttu-id="1d3d8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1d3d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d3d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d3d8-122">Authorization</span></span>|<span data-ttu-id="1d3d8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d3d8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1d3d8-124">Accept</span></span>|<span data-ttu-id="1d3d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d3d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d3d8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d3d8-126">Request body</span></span>
<span data-ttu-id="1d3d8-127">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="1d3d8-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="1d3d8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d3d8-129">Property</span></span>|<span data-ttu-id="1d3d8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1d3d8-130">Type</span></span>|<span data-ttu-id="1d3d8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1d3d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d3d8-132">id</span><span class="sxs-lookup"><span data-stu-id="1d3d8-132">id</span></span>|<span data-ttu-id="1d3d8-133">String</span><span class="sxs-lookup"><span data-stu-id="1d3d8-133">String</span></span>|<span data-ttu-id="1d3d8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-134">Key of the entity.</span></span> <span data-ttu-id="1d3d8-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d3d8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d3d8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d3d8-137">DateTimeOffset</span></span>|<span data-ttu-id="1d3d8-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d3d8-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d3d8-140">createdDateTime</span></span>|<span data-ttu-id="1d3d8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d3d8-141">DateTimeOffset</span></span>|<span data-ttu-id="1d3d8-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-142">DateTime the object was created.</span></span> <span data-ttu-id="1d3d8-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-144">description</span><span class="sxs-lookup"><span data-stu-id="1d3d8-144">description</span></span>|<span data-ttu-id="1d3d8-145">String</span><span class="sxs-lookup"><span data-stu-id="1d3d8-145">String</span></span>|<span data-ttu-id="1d3d8-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d3d8-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1d3d8-148">displayName</span></span>|<span data-ttu-id="1d3d8-149">String</span><span class="sxs-lookup"><span data-stu-id="1d3d8-149">String</span></span>|<span data-ttu-id="1d3d8-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d3d8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-152">version</span><span class="sxs-lookup"><span data-stu-id="1d3d8-152">version</span></span>|<span data-ttu-id="1d3d8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1d3d8-153">Int32</span></span>|<span data-ttu-id="1d3d8-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-154">Version of the device configuration.</span></span> <span data-ttu-id="1d3d8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d3d8-156">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="1d3d8-156">activeHoursStart</span></span>|<span data-ttu-id="1d3d8-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1d3d8-157">TimeOfDay</span></span>|<span data-ttu-id="1d3d8-158">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-158">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="1d3d8-159">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="1d3d8-159">activeHoursEnd</span></span>|<span data-ttu-id="1d3d8-160">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1d3d8-160">TimeOfDay</span></span>|<span data-ttu-id="1d3d8-161">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-161">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="1d3d8-162">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="1d3d8-162">scheduledInstallDays</span></span>|<span data-ttu-id="1d3d8-163">[коллекция dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="1d3d8-163">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="1d3d8-164">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-164">Days in week for which active hours are configured.</span></span> <span data-ttu-id="1d3d8-165">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-165">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1d3d8-166">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-166">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1d3d8-167">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d3d8-167">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="1d3d8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1d3d8-168">Int32</span></span>|<span data-ttu-id="1d3d8-169">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="1d3d8-169">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="1d3d8-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d3d8-170">Response</span></span>
<span data-ttu-id="1d3d8-171">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-171">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d3d8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="1d3d8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d3d8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d3d8-173">Request</span></span>
<span data-ttu-id="1d3d8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="1d3d8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d3d8-175">Response</span></span>
<span data-ttu-id="1d3d8-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d3d8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```




