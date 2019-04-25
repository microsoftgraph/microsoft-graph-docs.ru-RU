---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c4130b453cd2d18ee788afb4dcddc797be2719
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581508"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="b9a23-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9a23-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="b9a23-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9a23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a23-105">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9a23-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b9a23-106">Prerequisites</span></span>
<span data-ttu-id="b9a23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a23-109">Permission type</span></span>|<span data-ttu-id="b9a23-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9a23-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9a23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9a23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9a23-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9a23-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9a23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9a23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9a23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a23-114">Not supported.</span></span>|
|<span data-ttu-id="b9a23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9a23-115">Application</span></span>|<span data-ttu-id="b9a23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a23-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9a23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9a23-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9a23-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9a23-118">Request headers</span></span>
|<span data-ttu-id="b9a23-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9a23-119">Header</span></span>|<span data-ttu-id="b9a23-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b9a23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9a23-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9a23-121">Authorization</span></span>|<span data-ttu-id="b9a23-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9a23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9a23-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b9a23-123">Accept</span></span>|<span data-ttu-id="b9a23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b9a23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a23-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9a23-125">Request body</span></span>
<span data-ttu-id="b9a23-126">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9a23-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="b9a23-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="b9a23-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9a23-128">Property</span></span>|<span data-ttu-id="b9a23-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b9a23-129">Type</span></span>|<span data-ttu-id="b9a23-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a23-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a23-131">id</span><span class="sxs-lookup"><span data-stu-id="b9a23-131">id</span></span>|<span data-ttu-id="b9a23-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b9a23-132">String</span></span>|<span data-ttu-id="b9a23-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9a23-133">Key of the entity.</span></span> <span data-ttu-id="b9a23-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9a23-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b9a23-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9a23-136">DateTimeOffset</span></span>|<span data-ttu-id="b9a23-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b9a23-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b9a23-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9a23-139">createdDateTime</span></span>|<span data-ttu-id="b9a23-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9a23-140">DateTimeOffset</span></span>|<span data-ttu-id="b9a23-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b9a23-141">DateTime the object was created.</span></span> <span data-ttu-id="b9a23-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-143">description</span><span class="sxs-lookup"><span data-stu-id="b9a23-143">description</span></span>|<span data-ttu-id="b9a23-144">String</span><span class="sxs-lookup"><span data-stu-id="b9a23-144">String</span></span>|<span data-ttu-id="b9a23-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9a23-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9a23-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b9a23-147">displayName</span></span>|<span data-ttu-id="b9a23-148">String</span><span class="sxs-lookup"><span data-stu-id="b9a23-148">String</span></span>|<span data-ttu-id="b9a23-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9a23-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9a23-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9a23-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-151">version</span><span class="sxs-lookup"><span data-stu-id="b9a23-151">version</span></span>|<span data-ttu-id="b9a23-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b9a23-152">Int32</span></span>|<span data-ttu-id="b9a23-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9a23-153">Version of the device configuration.</span></span> <span data-ttu-id="b9a23-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9a23-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9a23-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="b9a23-155">allowSampleSharing</span></span>|<span data-ttu-id="b9a23-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9a23-156">Boolean</span></span>|<span data-ttu-id="b9a23-157">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="b9a23-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="b9a23-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="b9a23-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="b9a23-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9a23-159">Boolean</span></span>|<span data-ttu-id="b9a23-160">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="b9a23-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="b9a23-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a23-161">Response</span></span>
<span data-ttu-id="b9a23-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9a23-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a23-163">Пример</span><span class="sxs-lookup"><span data-stu-id="b9a23-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9a23-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9a23-164">Request</span></span>
<span data-ttu-id="b9a23-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9a23-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9a23-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a23-166">Response</span></span>
<span data-ttu-id="b9a23-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9a23-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



