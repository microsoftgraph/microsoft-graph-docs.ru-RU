---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3dba0ce2627735bc783f1f5e41c62aec1b5c681c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972189"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="b2f8a-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2f8a-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="b2f8a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2f8a-105">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2f8a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2f8a-106">Prerequisites</span></span>
<span data-ttu-id="b2f8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2f8a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f8a-109">Permission type</span></span>|<span data-ttu-id="b2f8a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2f8a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2f8a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2f8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2f8a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f8a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2f8a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2f8a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2f8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-114">Not supported.</span></span>|
|<span data-ttu-id="b2f8a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2f8a-115">Application</span></span>|<span data-ttu-id="b2f8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2f8a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2f8a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b2f8a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2f8a-118">Request headers</span></span>
|<span data-ttu-id="b2f8a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2f8a-119">Header</span></span>|<span data-ttu-id="b2f8a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b2f8a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2f8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2f8a-121">Authorization</span></span>|<span data-ttu-id="b2f8a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2f8a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2f8a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b2f8a-123">Accept</span></span>|<span data-ttu-id="b2f8a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2f8a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2f8a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2f8a-125">Request body</span></span>
<span data-ttu-id="b2f8a-126">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="b2f8a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="b2f8a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2f8a-128">Property</span></span>|<span data-ttu-id="b2f8a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b2f8a-129">Type</span></span>|<span data-ttu-id="b2f8a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b2f8a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f8a-131">id</span><span class="sxs-lookup"><span data-stu-id="b2f8a-131">id</span></span>|<span data-ttu-id="b2f8a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b2f8a-132">String</span></span>|<span data-ttu-id="b2f8a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-133">Key of the entity.</span></span> <span data-ttu-id="b2f8a-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2f8a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b2f8a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f8a-136">DateTimeOffset</span></span>|<span data-ttu-id="b2f8a-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b2f8a-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2f8a-139">createdDateTime</span></span>|<span data-ttu-id="b2f8a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f8a-140">DateTimeOffset</span></span>|<span data-ttu-id="b2f8a-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-141">DateTime the object was created.</span></span> <span data-ttu-id="b2f8a-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-143">описание</span><span class="sxs-lookup"><span data-stu-id="b2f8a-143">description</span></span>|<span data-ttu-id="b2f8a-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b2f8a-144">String</span></span>|<span data-ttu-id="b2f8a-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2f8a-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b2f8a-147">displayName</span></span>|<span data-ttu-id="b2f8a-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b2f8a-148">String</span></span>|<span data-ttu-id="b2f8a-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2f8a-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-151">version</span><span class="sxs-lookup"><span data-stu-id="b2f8a-151">version</span></span>|<span data-ttu-id="b2f8a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b2f8a-152">Int32</span></span>|<span data-ttu-id="b2f8a-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-153">Version of the device configuration.</span></span> <span data-ttu-id="b2f8a-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2f8a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2f8a-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="b2f8a-155">licenseType</span></span>|[<span data-ttu-id="b2f8a-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="b2f8a-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="b2f8a-157">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="b2f8a-158">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="b2f8a-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="b2f8a-159">targetEdition</span></span>|[<span data-ttu-id="b2f8a-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="b2f8a-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="b2f8a-161">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="b2f8a-162">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="b2f8a-163">license</span><span class="sxs-lookup"><span data-stu-id="b2f8a-163">license</span></span>|<span data-ttu-id="b2f8a-164">String</span><span class="sxs-lookup"><span data-stu-id="b2f8a-164">String</span></span>|<span data-ttu-id="b2f8a-165">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="b2f8a-166">productKey</span><span class="sxs-lookup"><span data-stu-id="b2f8a-166">productKey</span></span>|<span data-ttu-id="b2f8a-167">String</span><span class="sxs-lookup"><span data-stu-id="b2f8a-167">String</span></span>|<span data-ttu-id="b2f8a-168">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="b2f8a-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f8a-169">Response</span></span>
<span data-ttu-id="b2f8a-170">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2f8a-171">Пример</span><span class="sxs-lookup"><span data-stu-id="b2f8a-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2f8a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2f8a-172">Request</span></span>
<span data-ttu-id="b2f8a-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2f8a-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2f8a-174">Response</span></span>
<span data-ttu-id="b2f8a-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2f8a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



