---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2f7af8568f07403f4f2f337fb3fed6b9d876af4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261399"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="ca3f8-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca3f8-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="ca3f8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3f8-105">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca3f8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ca3f8-106">Prerequisites</span></span>
<span data-ttu-id="ca3f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca3f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3f8-109">Permission type</span></span>|<span data-ttu-id="ca3f8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca3f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca3f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca3f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca3f8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3f8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca3f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca3f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca3f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-114">Not supported.</span></span>|
|<span data-ttu-id="ca3f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca3f8-115">Application</span></span>|<span data-ttu-id="ca3f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca3f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca3f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca3f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca3f8-118">Request headers</span></span>
|<span data-ttu-id="ca3f8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca3f8-119">Header</span></span>|<span data-ttu-id="ca3f8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ca3f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca3f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca3f8-121">Authorization</span></span>|<span data-ttu-id="ca3f8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca3f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca3f8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ca3f8-123">Accept</span></span>|<span data-ttu-id="ca3f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca3f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca3f8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca3f8-125">Request body</span></span>
<span data-ttu-id="ca3f8-126">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="ca3f8-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="ca3f8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca3f8-128">Property</span></span>|<span data-ttu-id="ca3f8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ca3f8-129">Type</span></span>|<span data-ttu-id="ca3f8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ca3f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3f8-131">id</span><span class="sxs-lookup"><span data-stu-id="ca3f8-131">id</span></span>|<span data-ttu-id="ca3f8-132">String</span><span class="sxs-lookup"><span data-stu-id="ca3f8-132">String</span></span>|<span data-ttu-id="ca3f8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-133">Key of the entity.</span></span> <span data-ttu-id="ca3f8-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca3f8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ca3f8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca3f8-136">DateTimeOffset</span></span>|<span data-ttu-id="ca3f8-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ca3f8-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca3f8-139">createdDateTime</span></span>|<span data-ttu-id="ca3f8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca3f8-140">DateTimeOffset</span></span>|<span data-ttu-id="ca3f8-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-141">DateTime the object was created.</span></span> <span data-ttu-id="ca3f8-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-143">description</span><span class="sxs-lookup"><span data-stu-id="ca3f8-143">description</span></span>|<span data-ttu-id="ca3f8-144">String</span><span class="sxs-lookup"><span data-stu-id="ca3f8-144">String</span></span>|<span data-ttu-id="ca3f8-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca3f8-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ca3f8-147">displayName</span></span>|<span data-ttu-id="ca3f8-148">String</span><span class="sxs-lookup"><span data-stu-id="ca3f8-148">String</span></span>|<span data-ttu-id="ca3f8-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca3f8-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca3f8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-151">version</span><span class="sxs-lookup"><span data-stu-id="ca3f8-151">version</span></span>|<span data-ttu-id="ca3f8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ca3f8-152">Int32</span></span>|<span data-ttu-id="ca3f8-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-153">Version of the device configuration.</span></span> <span data-ttu-id="ca3f8-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f8-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="ca3f8-155">allowSampleSharing</span></span>|<span data-ttu-id="ca3f8-156">Логический</span><span class="sxs-lookup"><span data-stu-id="ca3f8-156">Boolean</span></span>|<span data-ttu-id="ca3f8-157">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="ca3f8-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="ca3f8-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="ca3f8-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="ca3f8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3f8-159">Boolean</span></span>|<span data-ttu-id="ca3f8-160">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="ca3f8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3f8-161">Response</span></span>
<span data-ttu-id="ca3f8-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca3f8-163">Пример</span><span class="sxs-lookup"><span data-stu-id="ca3f8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca3f8-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3f8-164">Request</span></span>
<span data-ttu-id="ca3f8-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="ca3f8-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca3f8-166">Response</span></span>
<span data-ttu-id="ca3f8-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ca3f8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



