---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72e3539e42dfc1ddc71252f1dea4ef09fadb1bfd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513838"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="902be-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="902be-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="902be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="902be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="902be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="902be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="902be-106">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="902be-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="902be-107">Prerequisites</span></span>
<span data-ttu-id="902be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="902be-110">Permission type</span></span>|<span data-ttu-id="902be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="902be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="902be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="902be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="902be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="902be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="902be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="902be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902be-115">Not supported.</span></span>|
|<span data-ttu-id="902be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="902be-116">Application</span></span>|<span data-ttu-id="902be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="902be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="902be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="902be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="902be-119">Request headers</span></span>
|<span data-ttu-id="902be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="902be-120">Header</span></span>|<span data-ttu-id="902be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="902be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="902be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="902be-122">Authorization</span></span>|<span data-ttu-id="902be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="902be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="902be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="902be-124">Accept</span></span>|<span data-ttu-id="902be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="902be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="902be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="902be-126">Request body</span></span>
<span data-ttu-id="902be-127">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902be-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="902be-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="902be-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="902be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="902be-129">Property</span></span>|<span data-ttu-id="902be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="902be-130">Type</span></span>|<span data-ttu-id="902be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="902be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="902be-132">id</span><span class="sxs-lookup"><span data-stu-id="902be-132">id</span></span>|<span data-ttu-id="902be-133">String</span><span class="sxs-lookup"><span data-stu-id="902be-133">String</span></span>|<span data-ttu-id="902be-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="902be-134">Key of the entity.</span></span> <span data-ttu-id="902be-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="902be-136">lastModifiedDateTime</span></span>|<span data-ttu-id="902be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="902be-137">DateTimeOffset</span></span>|<span data-ttu-id="902be-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="902be-138">DateTime the object was last modified.</span></span> <span data-ttu-id="902be-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="902be-140">createdDateTime</span></span>|<span data-ttu-id="902be-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="902be-141">DateTimeOffset</span></span>|<span data-ttu-id="902be-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="902be-142">DateTime the object was created.</span></span> <span data-ttu-id="902be-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-144">description</span><span class="sxs-lookup"><span data-stu-id="902be-144">description</span></span>|<span data-ttu-id="902be-145">String</span><span class="sxs-lookup"><span data-stu-id="902be-145">String</span></span>|<span data-ttu-id="902be-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="902be-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="902be-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-148">displayName</span><span class="sxs-lookup"><span data-stu-id="902be-148">displayName</span></span>|<span data-ttu-id="902be-149">Строка</span><span class="sxs-lookup"><span data-stu-id="902be-149">String</span></span>|<span data-ttu-id="902be-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="902be-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="902be-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="902be-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-152">version</span><span class="sxs-lookup"><span data-stu-id="902be-152">version</span></span>|<span data-ttu-id="902be-153">Int32</span><span class="sxs-lookup"><span data-stu-id="902be-153">Int32</span></span>|<span data-ttu-id="902be-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="902be-154">Version of the device configuration.</span></span> <span data-ttu-id="902be-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="902be-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="902be-156">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="902be-156">allowSampleSharing</span></span>|<span data-ttu-id="902be-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="902be-157">Boolean</span></span>|<span data-ttu-id="902be-158">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="902be-158">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="902be-159">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="902be-159">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="902be-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="902be-160">Boolean</span></span>|<span data-ttu-id="902be-161">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="902be-161">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="902be-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="902be-162">Response</span></span>
<span data-ttu-id="902be-163">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="902be-163">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="902be-164">Пример</span><span class="sxs-lookup"><span data-stu-id="902be-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="902be-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="902be-165">Request</span></span>
<span data-ttu-id="902be-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="902be-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="902be-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="902be-167">Response</span></span>
<span data-ttu-id="902be-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="902be-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




