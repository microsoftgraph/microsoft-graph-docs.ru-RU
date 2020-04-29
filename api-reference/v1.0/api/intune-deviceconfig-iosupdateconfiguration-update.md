---
title: Обновление объекта iosUpdateConfiguration
description: Обновление свойств объекта iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b41eed80f91122865b49d0f6f1c091c524ec6658
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454236"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="f3f07-103">Обновление объекта iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3f07-103">Update iosUpdateConfiguration</span></span>

<span data-ttu-id="f3f07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3f07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3f07-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3f07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f07-106">Обновление свойств объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3f07-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3f07-107">Prerequisites</span></span>
<span data-ttu-id="f3f07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3f07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3f07-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f07-110">Permission type</span></span>|<span data-ttu-id="f3f07-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3f07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3f07-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3f07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3f07-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3f07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f07-115">Not supported.</span></span>|
|<span data-ttu-id="f3f07-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3f07-116">Application</span></span>|<span data-ttu-id="f3f07-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3f07-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3f07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f3f07-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3f07-119">Request headers</span></span>
|<span data-ttu-id="f3f07-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3f07-120">Header</span></span>|<span data-ttu-id="f3f07-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3f07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3f07-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3f07-122">Authorization</span></span>|<span data-ttu-id="f3f07-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3f07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3f07-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f3f07-124">Accept</span></span>|<span data-ttu-id="f3f07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3f07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f07-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3f07-126">Request body</span></span>
<span data-ttu-id="f3f07-127">В теле запроса добавьте представление объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3f07-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="f3f07-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="f3f07-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3f07-129">Property</span></span>|<span data-ttu-id="f3f07-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f3f07-130">Type</span></span>|<span data-ttu-id="f3f07-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f07-132">id</span><span class="sxs-lookup"><span data-stu-id="f3f07-132">id</span></span>|<span data-ttu-id="f3f07-133">String</span><span class="sxs-lookup"><span data-stu-id="f3f07-133">String</span></span>|<span data-ttu-id="f3f07-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3f07-134">Key of the entity.</span></span> <span data-ttu-id="f3f07-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f07-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f3f07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f07-137">DateTimeOffset</span></span>|<span data-ttu-id="f3f07-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f3f07-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f3f07-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f07-140">createdDateTime</span></span>|<span data-ttu-id="f3f07-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f07-141">DateTimeOffset</span></span>|<span data-ttu-id="f3f07-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f3f07-142">DateTime the object was created.</span></span> <span data-ttu-id="f3f07-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-144">description</span><span class="sxs-lookup"><span data-stu-id="f3f07-144">description</span></span>|<span data-ttu-id="f3f07-145">String</span><span class="sxs-lookup"><span data-stu-id="f3f07-145">String</span></span>|<span data-ttu-id="f3f07-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3f07-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3f07-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f3f07-148">displayName</span></span>|<span data-ttu-id="f3f07-149">Строка</span><span class="sxs-lookup"><span data-stu-id="f3f07-149">String</span></span>|<span data-ttu-id="f3f07-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3f07-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3f07-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3f07-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-152">version</span><span class="sxs-lookup"><span data-stu-id="f3f07-152">version</span></span>|<span data-ttu-id="f3f07-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f3f07-153">Int32</span></span>|<span data-ttu-id="f3f07-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3f07-154">Version of the device configuration.</span></span> <span data-ttu-id="f3f07-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3f07-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3f07-156">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="f3f07-156">activeHoursStart</span></span>|<span data-ttu-id="f3f07-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3f07-157">TimeOfDay</span></span>|<span data-ttu-id="f3f07-158">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="f3f07-158">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="f3f07-159">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="f3f07-159">activeHoursEnd</span></span>|<span data-ttu-id="f3f07-160">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3f07-160">TimeOfDay</span></span>|<span data-ttu-id="f3f07-161">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="f3f07-161">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="f3f07-162">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="f3f07-162">scheduledInstallDays</span></span>|<span data-ttu-id="f3f07-163">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="f3f07-163">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="f3f07-164">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="f3f07-164">Days in week for which active hours are configured.</span></span> <span data-ttu-id="f3f07-165">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="f3f07-165">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="f3f07-166">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f3f07-166">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f3f07-167">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="f3f07-167">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="f3f07-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f3f07-168">Int32</span></span>|<span data-ttu-id="f3f07-169">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="f3f07-169">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="f3f07-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f07-170">Response</span></span>
<span data-ttu-id="f3f07-171">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3f07-171">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3f07-172">Пример</span><span class="sxs-lookup"><span data-stu-id="f3f07-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3f07-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3f07-173">Request</span></span>
<span data-ttu-id="f3f07-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3f07-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f3f07-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f07-175">Response</span></span>
<span data-ttu-id="f3f07-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3f07-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






