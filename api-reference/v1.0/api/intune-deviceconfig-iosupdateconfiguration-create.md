---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 400db047bdc4c4118d38e915cf90e8481d7d02dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806960"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="4251b-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="4251b-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="4251b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4251b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4251b-105">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4251b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4251b-106">Prerequisites</span></span>
<span data-ttu-id="4251b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4251b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4251b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4251b-109">Permission type</span></span>|<span data-ttu-id="4251b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4251b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4251b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4251b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4251b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4251b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4251b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4251b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4251b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4251b-114">Not supported.</span></span>|
|<span data-ttu-id="4251b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4251b-115">Application</span></span>|<span data-ttu-id="4251b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4251b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4251b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4251b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4251b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4251b-118">Request headers</span></span>
|<span data-ttu-id="4251b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4251b-119">Header</span></span>|<span data-ttu-id="4251b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4251b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4251b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4251b-121">Authorization</span></span>|<span data-ttu-id="4251b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4251b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4251b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4251b-123">Accept</span></span>|<span data-ttu-id="4251b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4251b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4251b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4251b-125">Request body</span></span>
<span data-ttu-id="4251b-126">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4251b-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="4251b-127">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4251b-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="4251b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4251b-128">Property</span></span>|<span data-ttu-id="4251b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4251b-129">Type</span></span>|<span data-ttu-id="4251b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4251b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4251b-131">id</span><span class="sxs-lookup"><span data-stu-id="4251b-131">id</span></span>|<span data-ttu-id="4251b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4251b-132">String</span></span>|<span data-ttu-id="4251b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4251b-133">Key of the entity.</span></span> <span data-ttu-id="4251b-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4251b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4251b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4251b-136">DateTimeOffset</span></span>|<span data-ttu-id="4251b-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4251b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4251b-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4251b-139">createdDateTime</span></span>|<span data-ttu-id="4251b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4251b-140">DateTimeOffset</span></span>|<span data-ttu-id="4251b-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4251b-141">DateTime the object was created.</span></span> <span data-ttu-id="4251b-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-143">описание</span><span class="sxs-lookup"><span data-stu-id="4251b-143">description</span></span>|<span data-ttu-id="4251b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="4251b-144">String</span></span>|<span data-ttu-id="4251b-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4251b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4251b-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4251b-147">displayName</span></span>|<span data-ttu-id="4251b-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4251b-148">String</span></span>|<span data-ttu-id="4251b-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4251b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4251b-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-151">version</span><span class="sxs-lookup"><span data-stu-id="4251b-151">version</span></span>|<span data-ttu-id="4251b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4251b-152">Int32</span></span>|<span data-ttu-id="4251b-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4251b-153">Version of the device configuration.</span></span> <span data-ttu-id="4251b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4251b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4251b-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="4251b-155">activeHoursStart</span></span>|<span data-ttu-id="4251b-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4251b-156">TimeOfDay</span></span>|<span data-ttu-id="4251b-157">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="4251b-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="4251b-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="4251b-158">activeHoursEnd</span></span>|<span data-ttu-id="4251b-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4251b-159">TimeOfDay</span></span>|<span data-ttu-id="4251b-160">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="4251b-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="4251b-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="4251b-161">scheduledInstallDays</span></span>|<span data-ttu-id="4251b-162">Коллекция [dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="4251b-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="4251b-163">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="4251b-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="4251b-164">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="4251b-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="4251b-165">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4251b-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4251b-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="4251b-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="4251b-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4251b-167">Int32</span></span>|<span data-ttu-id="4251b-168">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="4251b-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="4251b-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="4251b-169">Response</span></span>
<span data-ttu-id="4251b-170">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4251b-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4251b-171">Пример</span><span class="sxs-lookup"><span data-stu-id="4251b-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="4251b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4251b-172">Request</span></span>
<span data-ttu-id="4251b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4251b-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4251b-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="4251b-174">Response</span></span>
<span data-ttu-id="4251b-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4251b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



