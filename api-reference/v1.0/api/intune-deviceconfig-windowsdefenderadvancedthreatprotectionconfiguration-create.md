---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 31db5f1c254ebe5721748c4e8f35907c49b72217
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355505"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="bd357-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd357-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="bd357-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bd357-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd357-105">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd357-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bd357-106">Prerequisites</span></span>
<span data-ttu-id="bd357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd357-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd357-109">Permission type</span></span>|<span data-ttu-id="bd357-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd357-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd357-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd357-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd357-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd357-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd357-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd357-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd357-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd357-114">Not supported.</span></span>|
|<span data-ttu-id="bd357-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd357-115">Application</span></span>|<span data-ttu-id="bd357-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd357-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd357-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd357-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd357-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd357-118">Request headers</span></span>
|<span data-ttu-id="bd357-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd357-119">Header</span></span>|<span data-ttu-id="bd357-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bd357-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd357-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd357-121">Authorization</span></span>|<span data-ttu-id="bd357-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd357-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd357-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bd357-123">Accept</span></span>|<span data-ttu-id="bd357-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd357-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd357-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd357-125">Request body</span></span>
<span data-ttu-id="bd357-126">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd357-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="bd357-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd357-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="bd357-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd357-128">Property</span></span>|<span data-ttu-id="bd357-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bd357-129">Type</span></span>|<span data-ttu-id="bd357-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd357-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd357-131">id</span><span class="sxs-lookup"><span data-stu-id="bd357-131">id</span></span>|<span data-ttu-id="bd357-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bd357-132">String</span></span>|<span data-ttu-id="bd357-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd357-133">Key of the entity.</span></span> <span data-ttu-id="bd357-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd357-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bd357-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd357-136">DateTimeOffset</span></span>|<span data-ttu-id="bd357-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bd357-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bd357-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd357-139">createdDateTime</span></span>|<span data-ttu-id="bd357-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd357-140">DateTimeOffset</span></span>|<span data-ttu-id="bd357-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bd357-141">DateTime the object was created.</span></span> <span data-ttu-id="bd357-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-143">описание</span><span class="sxs-lookup"><span data-stu-id="bd357-143">description</span></span>|<span data-ttu-id="bd357-144">Строка</span><span class="sxs-lookup"><span data-stu-id="bd357-144">String</span></span>|<span data-ttu-id="bd357-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd357-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd357-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bd357-147">displayName</span></span>|<span data-ttu-id="bd357-148">Строка</span><span class="sxs-lookup"><span data-stu-id="bd357-148">String</span></span>|<span data-ttu-id="bd357-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd357-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd357-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd357-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-151">version</span><span class="sxs-lookup"><span data-stu-id="bd357-151">version</span></span>|<span data-ttu-id="bd357-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bd357-152">Int32</span></span>|<span data-ttu-id="bd357-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bd357-153">Version of the device configuration.</span></span> <span data-ttu-id="bd357-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd357-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bd357-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="bd357-155">allowSampleSharing</span></span>|<span data-ttu-id="bd357-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd357-156">Boolean</span></span>|<span data-ttu-id="bd357-157">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="bd357-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="bd357-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="bd357-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="bd357-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd357-159">Boolean</span></span>|<span data-ttu-id="bd357-160">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="bd357-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="bd357-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd357-161">Response</span></span>
<span data-ttu-id="bd357-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bd357-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd357-163">Пример</span><span class="sxs-lookup"><span data-stu-id="bd357-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd357-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd357-164">Request</span></span>
<span data-ttu-id="bd357-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd357-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd357-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd357-166">Response</span></span>
<span data-ttu-id="bd357-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd357-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



