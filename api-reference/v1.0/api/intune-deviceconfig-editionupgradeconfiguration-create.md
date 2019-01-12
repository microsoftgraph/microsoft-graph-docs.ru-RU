---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c32873ffe50a4a35f94324d782e055508389e7e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937924"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="458c6-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="458c6-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="458c6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="458c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="458c6-105">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="458c6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="458c6-106">Prerequisites</span></span>
<span data-ttu-id="458c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="458c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="458c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="458c6-109">Permission type</span></span>|<span data-ttu-id="458c6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="458c6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="458c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="458c6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="458c6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="458c6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="458c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="458c6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="458c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="458c6-114">Not supported.</span></span>|
|<span data-ttu-id="458c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="458c6-115">Application</span></span>|<span data-ttu-id="458c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="458c6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="458c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="458c6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="458c6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="458c6-118">Request headers</span></span>
|<span data-ttu-id="458c6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="458c6-119">Header</span></span>|<span data-ttu-id="458c6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="458c6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="458c6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="458c6-121">Authorization</span></span>|<span data-ttu-id="458c6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="458c6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="458c6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="458c6-123">Accept</span></span>|<span data-ttu-id="458c6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="458c6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="458c6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="458c6-125">Request body</span></span>
<span data-ttu-id="458c6-126">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="458c6-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="458c6-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="458c6-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="458c6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="458c6-128">Property</span></span>|<span data-ttu-id="458c6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="458c6-129">Type</span></span>|<span data-ttu-id="458c6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="458c6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="458c6-131">id</span><span class="sxs-lookup"><span data-stu-id="458c6-131">id</span></span>|<span data-ttu-id="458c6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="458c6-132">String</span></span>|<span data-ttu-id="458c6-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="458c6-133">Key of the entity.</span></span> <span data-ttu-id="458c6-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="458c6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="458c6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="458c6-136">DateTimeOffset</span></span>|<span data-ttu-id="458c6-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="458c6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="458c6-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="458c6-139">createdDateTime</span></span>|<span data-ttu-id="458c6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="458c6-140">DateTimeOffset</span></span>|<span data-ttu-id="458c6-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="458c6-141">DateTime the object was created.</span></span> <span data-ttu-id="458c6-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-143">описание</span><span class="sxs-lookup"><span data-stu-id="458c6-143">description</span></span>|<span data-ttu-id="458c6-144">Строка</span><span class="sxs-lookup"><span data-stu-id="458c6-144">String</span></span>|<span data-ttu-id="458c6-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="458c6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="458c6-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="458c6-147">displayName</span></span>|<span data-ttu-id="458c6-148">Строка</span><span class="sxs-lookup"><span data-stu-id="458c6-148">String</span></span>|<span data-ttu-id="458c6-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="458c6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="458c6-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-151">version</span><span class="sxs-lookup"><span data-stu-id="458c6-151">version</span></span>|<span data-ttu-id="458c6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="458c6-152">Int32</span></span>|<span data-ttu-id="458c6-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="458c6-153">Version of the device configuration.</span></span> <span data-ttu-id="458c6-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="458c6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="458c6-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="458c6-155">licenseType</span></span>|[<span data-ttu-id="458c6-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="458c6-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="458c6-157">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="458c6-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="458c6-158">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="458c6-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="458c6-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="458c6-159">targetEdition</span></span>|[<span data-ttu-id="458c6-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="458c6-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="458c6-161">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="458c6-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="458c6-162">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="458c6-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="458c6-163">license</span><span class="sxs-lookup"><span data-stu-id="458c6-163">license</span></span>|<span data-ttu-id="458c6-164">String</span><span class="sxs-lookup"><span data-stu-id="458c6-164">String</span></span>|<span data-ttu-id="458c6-165">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="458c6-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="458c6-166">productKey</span><span class="sxs-lookup"><span data-stu-id="458c6-166">productKey</span></span>|<span data-ttu-id="458c6-167">String</span><span class="sxs-lookup"><span data-stu-id="458c6-167">String</span></span>|<span data-ttu-id="458c6-168">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="458c6-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="458c6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="458c6-169">Response</span></span>
<span data-ttu-id="458c6-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="458c6-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="458c6-171">Пример</span><span class="sxs-lookup"><span data-stu-id="458c6-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="458c6-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="458c6-172">Request</span></span>
<span data-ttu-id="458c6-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="458c6-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="458c6-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="458c6-174">Response</span></span>
<span data-ttu-id="458c6-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="458c6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



