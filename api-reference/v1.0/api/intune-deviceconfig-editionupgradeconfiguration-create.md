---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ff46afb29b9ece823e9115bd580fc6ca258135a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368514"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="f43c5-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f43c5-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="f43c5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f43c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f43c5-105">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f43c5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f43c5-106">Prerequisites</span></span>
<span data-ttu-id="f43c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f43c5-109">Permission type</span></span>|<span data-ttu-id="f43c5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f43c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f43c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f43c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f43c5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f43c5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f43c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f43c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f43c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f43c5-114">Not supported.</span></span>|
|<span data-ttu-id="f43c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f43c5-115">Application</span></span>|<span data-ttu-id="f43c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f43c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f43c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f43c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f43c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f43c5-118">Request headers</span></span>
|<span data-ttu-id="f43c5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f43c5-119">Header</span></span>|<span data-ttu-id="f43c5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f43c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f43c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f43c5-121">Authorization</span></span>|<span data-ttu-id="f43c5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f43c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f43c5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f43c5-123">Accept</span></span>|<span data-ttu-id="f43c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f43c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f43c5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f43c5-125">Request body</span></span>
<span data-ttu-id="f43c5-126">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f43c5-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="f43c5-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f43c5-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="f43c5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f43c5-128">Property</span></span>|<span data-ttu-id="f43c5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f43c5-129">Type</span></span>|<span data-ttu-id="f43c5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f43c5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f43c5-131">id</span><span class="sxs-lookup"><span data-stu-id="f43c5-131">id</span></span>|<span data-ttu-id="f43c5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f43c5-132">String</span></span>|<span data-ttu-id="f43c5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f43c5-133">Key of the entity.</span></span> <span data-ttu-id="f43c5-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f43c5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f43c5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43c5-136">DateTimeOffset</span></span>|<span data-ttu-id="f43c5-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f43c5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f43c5-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f43c5-139">createdDateTime</span></span>|<span data-ttu-id="f43c5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43c5-140">DateTimeOffset</span></span>|<span data-ttu-id="f43c5-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f43c5-141">DateTime the object was created.</span></span> <span data-ttu-id="f43c5-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-143">description</span><span class="sxs-lookup"><span data-stu-id="f43c5-143">description</span></span>|<span data-ttu-id="f43c5-144">String</span><span class="sxs-lookup"><span data-stu-id="f43c5-144">String</span></span>|<span data-ttu-id="f43c5-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f43c5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f43c5-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f43c5-147">displayName</span></span>|<span data-ttu-id="f43c5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="f43c5-148">String</span></span>|<span data-ttu-id="f43c5-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f43c5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f43c5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f43c5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-151">version</span><span class="sxs-lookup"><span data-stu-id="f43c5-151">version</span></span>|<span data-ttu-id="f43c5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f43c5-152">Int32</span></span>|<span data-ttu-id="f43c5-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f43c5-153">Version of the device configuration.</span></span> <span data-ttu-id="f43c5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f43c5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f43c5-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="f43c5-155">licenseType</span></span>|[<span data-ttu-id="f43c5-156">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="f43c5-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="f43c5-157">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f43c5-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="f43c5-158">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="f43c5-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="f43c5-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="f43c5-159">targetEdition</span></span>|[<span data-ttu-id="f43c5-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="f43c5-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="f43c5-161">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="f43c5-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="f43c5-162">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="f43c5-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="f43c5-163">license</span><span class="sxs-lookup"><span data-stu-id="f43c5-163">license</span></span>|<span data-ttu-id="f43c5-164">String</span><span class="sxs-lookup"><span data-stu-id="f43c5-164">String</span></span>|<span data-ttu-id="f43c5-165">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f43c5-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="f43c5-166">productKey</span><span class="sxs-lookup"><span data-stu-id="f43c5-166">productKey</span></span>|<span data-ttu-id="f43c5-167">String</span><span class="sxs-lookup"><span data-stu-id="f43c5-167">String</span></span>|<span data-ttu-id="f43c5-168">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f43c5-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="f43c5-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="f43c5-169">Response</span></span>
<span data-ttu-id="f43c5-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f43c5-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f43c5-171">Пример</span><span class="sxs-lookup"><span data-stu-id="f43c5-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f43c5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f43c5-172">Request</span></span>
<span data-ttu-id="f43c5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f43c5-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f43c5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f43c5-174">Response</span></span>
<span data-ttu-id="f43c5-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f43c5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




