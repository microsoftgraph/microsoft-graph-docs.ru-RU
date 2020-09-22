---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4565ff1e816c85c7a850d685729e0677bd67edf5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045777"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="cc103-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc103-103">Create editionUpgradeConfiguration</span></span>

<span data-ttu-id="cc103-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc103-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc103-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc103-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc103-106">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc103-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cc103-107">Prerequisites</span></span>
<span data-ttu-id="cc103-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc103-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc103-110">Permission type</span></span>|<span data-ttu-id="cc103-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc103-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc103-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc103-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc103-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc103-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc103-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc103-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc103-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc103-115">Not supported.</span></span>|
|<span data-ttu-id="cc103-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc103-116">Application</span></span>|<span data-ttu-id="cc103-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc103-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc103-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc103-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cc103-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc103-119">Request headers</span></span>
|<span data-ttu-id="cc103-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc103-120">Header</span></span>|<span data-ttu-id="cc103-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc103-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc103-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc103-122">Authorization</span></span>|<span data-ttu-id="cc103-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc103-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc103-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc103-124">Accept</span></span>|<span data-ttu-id="cc103-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc103-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc103-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc103-126">Request body</span></span>
<span data-ttu-id="cc103-127">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc103-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="cc103-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cc103-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="cc103-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc103-129">Property</span></span>|<span data-ttu-id="cc103-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc103-130">Type</span></span>|<span data-ttu-id="cc103-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc103-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc103-132">id</span><span class="sxs-lookup"><span data-stu-id="cc103-132">id</span></span>|<span data-ttu-id="cc103-133">String</span><span class="sxs-lookup"><span data-stu-id="cc103-133">String</span></span>|<span data-ttu-id="cc103-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cc103-134">Key of the entity.</span></span> <span data-ttu-id="cc103-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc103-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cc103-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc103-137">DateTimeOffset</span></span>|<span data-ttu-id="cc103-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cc103-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cc103-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc103-140">createdDateTime</span></span>|<span data-ttu-id="cc103-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc103-141">DateTimeOffset</span></span>|<span data-ttu-id="cc103-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cc103-142">DateTime the object was created.</span></span> <span data-ttu-id="cc103-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-144">description</span><span class="sxs-lookup"><span data-stu-id="cc103-144">description</span></span>|<span data-ttu-id="cc103-145">String</span><span class="sxs-lookup"><span data-stu-id="cc103-145">String</span></span>|<span data-ttu-id="cc103-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc103-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc103-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-148">displayName</span><span class="sxs-lookup"><span data-stu-id="cc103-148">displayName</span></span>|<span data-ttu-id="cc103-149">String</span><span class="sxs-lookup"><span data-stu-id="cc103-149">String</span></span>|<span data-ttu-id="cc103-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc103-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc103-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-152">version</span><span class="sxs-lookup"><span data-stu-id="cc103-152">version</span></span>|<span data-ttu-id="cc103-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cc103-153">Int32</span></span>|<span data-ttu-id="cc103-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc103-154">Version of the device configuration.</span></span> <span data-ttu-id="cc103-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc103-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc103-156">licenseType</span><span class="sxs-lookup"><span data-stu-id="cc103-156">licenseType</span></span>|[<span data-ttu-id="cc103-157">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="cc103-157">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="cc103-158">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="cc103-158">Edition Upgrade License Type.</span></span> <span data-ttu-id="cc103-159">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="cc103-159">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="cc103-160">targetEdition</span><span class="sxs-lookup"><span data-stu-id="cc103-160">targetEdition</span></span>|[<span data-ttu-id="cc103-161">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="cc103-161">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="cc103-162">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="cc103-162">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="cc103-163">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="cc103-163">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="cc103-164">license</span><span class="sxs-lookup"><span data-stu-id="cc103-164">license</span></span>|<span data-ttu-id="cc103-165">String</span><span class="sxs-lookup"><span data-stu-id="cc103-165">String</span></span>|<span data-ttu-id="cc103-166">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="cc103-166">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="cc103-167">productKey</span><span class="sxs-lookup"><span data-stu-id="cc103-167">productKey</span></span>|<span data-ttu-id="cc103-168">String</span><span class="sxs-lookup"><span data-stu-id="cc103-168">String</span></span>|<span data-ttu-id="cc103-169">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="cc103-169">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="cc103-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc103-170">Response</span></span>
<span data-ttu-id="cc103-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cc103-171">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc103-172">Пример</span><span class="sxs-lookup"><span data-stu-id="cc103-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc103-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc103-173">Request</span></span>
<span data-ttu-id="cc103-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc103-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="cc103-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc103-175">Response</span></span>
<span data-ttu-id="cc103-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc103-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









