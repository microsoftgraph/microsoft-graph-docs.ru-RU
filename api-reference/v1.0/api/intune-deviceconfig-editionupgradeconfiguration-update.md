---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59f379b93ccb49979b08837316feb80d0b0e2a0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514664"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="08300-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="08300-103">Update editionUpgradeConfiguration</span></span>

<span data-ttu-id="08300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08300-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08300-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08300-106">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08300-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08300-107">Prerequisites</span></span>
<span data-ttu-id="08300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08300-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08300-110">Permission type</span></span>|<span data-ttu-id="08300-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08300-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08300-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08300-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08300-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08300-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08300-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08300-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08300-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08300-115">Not supported.</span></span>|
|<span data-ttu-id="08300-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08300-116">Application</span></span>|<span data-ttu-id="08300-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08300-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08300-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08300-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="08300-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08300-119">Request headers</span></span>
|<span data-ttu-id="08300-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08300-120">Header</span></span>|<span data-ttu-id="08300-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08300-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08300-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08300-122">Authorization</span></span>|<span data-ttu-id="08300-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08300-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08300-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08300-124">Accept</span></span>|<span data-ttu-id="08300-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08300-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08300-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08300-126">Request body</span></span>
<span data-ttu-id="08300-127">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08300-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="08300-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="08300-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08300-129">Property</span></span>|<span data-ttu-id="08300-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08300-130">Type</span></span>|<span data-ttu-id="08300-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08300-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08300-132">id</span><span class="sxs-lookup"><span data-stu-id="08300-132">id</span></span>|<span data-ttu-id="08300-133">Строка</span><span class="sxs-lookup"><span data-stu-id="08300-133">String</span></span>|<span data-ttu-id="08300-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08300-134">Key of the entity.</span></span> <span data-ttu-id="08300-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08300-136">lastModifiedDateTime</span></span>|<span data-ttu-id="08300-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08300-137">DateTimeOffset</span></span>|<span data-ttu-id="08300-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="08300-138">DateTime the object was last modified.</span></span> <span data-ttu-id="08300-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08300-140">createdDateTime</span></span>|<span data-ttu-id="08300-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08300-141">DateTimeOffset</span></span>|<span data-ttu-id="08300-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="08300-142">DateTime the object was created.</span></span> <span data-ttu-id="08300-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-144">description</span><span class="sxs-lookup"><span data-stu-id="08300-144">description</span></span>|<span data-ttu-id="08300-145">String</span><span class="sxs-lookup"><span data-stu-id="08300-145">String</span></span>|<span data-ttu-id="08300-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08300-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08300-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-148">displayName</span><span class="sxs-lookup"><span data-stu-id="08300-148">displayName</span></span>|<span data-ttu-id="08300-149">Строка</span><span class="sxs-lookup"><span data-stu-id="08300-149">String</span></span>|<span data-ttu-id="08300-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08300-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08300-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08300-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-152">version</span><span class="sxs-lookup"><span data-stu-id="08300-152">version</span></span>|<span data-ttu-id="08300-153">Int32</span><span class="sxs-lookup"><span data-stu-id="08300-153">Int32</span></span>|<span data-ttu-id="08300-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08300-154">Version of the device configuration.</span></span> <span data-ttu-id="08300-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08300-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08300-156">licenseType</span><span class="sxs-lookup"><span data-stu-id="08300-156">licenseType</span></span>|[<span data-ttu-id="08300-157">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="08300-157">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="08300-158">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="08300-158">Edition Upgrade License Type.</span></span> <span data-ttu-id="08300-159">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="08300-159">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="08300-160">targetEdition</span><span class="sxs-lookup"><span data-stu-id="08300-160">targetEdition</span></span>|[<span data-ttu-id="08300-161">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="08300-161">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="08300-162">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="08300-162">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="08300-163">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="08300-163">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="08300-164">license</span><span class="sxs-lookup"><span data-stu-id="08300-164">license</span></span>|<span data-ttu-id="08300-165">String</span><span class="sxs-lookup"><span data-stu-id="08300-165">String</span></span>|<span data-ttu-id="08300-166">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="08300-166">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="08300-167">productKey</span><span class="sxs-lookup"><span data-stu-id="08300-167">productKey</span></span>|<span data-ttu-id="08300-168">String</span><span class="sxs-lookup"><span data-stu-id="08300-168">String</span></span>|<span data-ttu-id="08300-169">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="08300-169">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="08300-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="08300-170">Response</span></span>
<span data-ttu-id="08300-171">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08300-171">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08300-172">Пример</span><span class="sxs-lookup"><span data-stu-id="08300-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="08300-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="08300-173">Request</span></span>
<span data-ttu-id="08300-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08300-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="08300-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="08300-175">Response</span></span>
<span data-ttu-id="08300-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08300-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```




