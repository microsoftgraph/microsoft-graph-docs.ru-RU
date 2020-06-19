---
title: Обновление Андроиддевицеовнертрустедрутцертификате
description: Обновление свойств объекта Андроиддевицеовнертрустедрутцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df01b5964f1ba672a729db74a089423234d485ca
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793061"
---
# <a name="update-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="b1b0f-103">Обновление Андроиддевицеовнертрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="b1b0f-103">Update androidDeviceOwnerTrustedRootCertificate</span></span>

<span data-ttu-id="b1b0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1b0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1b0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b0f-107">Обновление свойств объекта [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b1b0f-107">Update the properties of a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1b0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1b0f-108">Prerequisites</span></span>
<span data-ttu-id="b1b0f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b1b0f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1b0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1b0f-111">Permission type</span></span>|<span data-ttu-id="b1b0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1b0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1b0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1b0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1b0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1b0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1b0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1b0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-116">Not supported.</span></span>|
|<span data-ttu-id="b1b0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1b0f-117">Application</span></span>|<span data-ttu-id="b1b0f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b0f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1b0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1b0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b1b0f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1b0f-120">Request headers</span></span>
|<span data-ttu-id="b1b0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1b0f-121">Header</span></span>|<span data-ttu-id="b1b0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1b0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1b0f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1b0f-123">Authorization</span></span>|<span data-ttu-id="b1b0f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1b0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1b0f-125">Accept</span></span>|<span data-ttu-id="b1b0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1b0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1b0f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1b0f-127">Request body</span></span>
<span data-ttu-id="b1b0f-128">В тексте запроса добавьте представление объекта [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-128">In the request body, supply a JSON representation for the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="b1b0f-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-129">The following table shows the properties that are required when you create the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span></span>

|<span data-ttu-id="b1b0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1b0f-130">Property</span></span>|<span data-ttu-id="b1b0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1b0f-131">Type</span></span>|<span data-ttu-id="b1b0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b0f-133">id</span><span class="sxs-lookup"><span data-stu-id="b1b0f-133">id</span></span>|<span data-ttu-id="b1b0f-134">String</span><span class="sxs-lookup"><span data-stu-id="b1b0f-134">String</span></span>|<span data-ttu-id="b1b0f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-135">Key of the entity.</span></span> <span data-ttu-id="b1b0f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b0f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b1b0f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b0f-138">DateTimeOffset</span></span>|<span data-ttu-id="b1b0f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b1b0f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1b0f-141">roleScopeTagIds</span></span>|<span data-ttu-id="b1b0f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1b0f-142">String collection</span></span>|<span data-ttu-id="b1b0f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1b0f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b1b0f-145">supportsScopeTags</span></span>|<span data-ttu-id="b1b0f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1b0f-146">Boolean</span></span>|<span data-ttu-id="b1b0f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1b0f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1b0f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1b0f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-150">This property is read-only.</span></span> <span data-ttu-id="b1b0f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1b0f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1b0f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1b0f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1b0f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b1b0f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1b0f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1b0f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1b0f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1b0f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b1b0f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1b0f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1b0f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1b0f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1b0f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b1b0f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b0f-164">createdDateTime</span></span>|<span data-ttu-id="b1b0f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b0f-165">DateTimeOffset</span></span>|<span data-ttu-id="b1b0f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-166">DateTime the object was created.</span></span> <span data-ttu-id="b1b0f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-168">description</span><span class="sxs-lookup"><span data-stu-id="b1b0f-168">description</span></span>|<span data-ttu-id="b1b0f-169">String</span><span class="sxs-lookup"><span data-stu-id="b1b0f-169">String</span></span>|<span data-ttu-id="b1b0f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1b0f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b1b0f-172">displayName</span></span>|<span data-ttu-id="b1b0f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b1b0f-173">String</span></span>|<span data-ttu-id="b1b0f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1b0f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-176">version</span><span class="sxs-lookup"><span data-stu-id="b1b0f-176">version</span></span>|<span data-ttu-id="b1b0f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b0f-177">Int32</span></span>|<span data-ttu-id="b1b0f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-178">Version of the device configuration.</span></span> <span data-ttu-id="b1b0f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1b0f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1b0f-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b1b0f-180">trustedRootCertificate</span></span>|<span data-ttu-id="b1b0f-181">Binary</span><span class="sxs-lookup"><span data-stu-id="b1b0f-181">Binary</span></span>|<span data-ttu-id="b1b0f-182">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="b1b0f-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="b1b0f-183">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="b1b0f-183">certFileName</span></span>|<span data-ttu-id="b1b0f-184">String</span><span class="sxs-lookup"><span data-stu-id="b1b0f-184">String</span></span>|<span data-ttu-id="b1b0f-185">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="b1b0f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b0f-186">Response</span></span>
<span data-ttu-id="b1b0f-187">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-187">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b0f-188">Пример</span><span class="sxs-lookup"><span data-stu-id="b1b0f-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1b0f-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1b0f-189">Request</span></span>
<span data-ttu-id="b1b0f-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="b1b0f-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b0f-191">Response</span></span>
<span data-ttu-id="b1b0f-192">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-192">Here is an example of the response.</span></span> <span data-ttu-id="b1b0f-193">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1b0f-194">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b1b0f-194">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
  "id": "6efc1a55-1a55-6efc-551a-fc6e551afc6e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```



