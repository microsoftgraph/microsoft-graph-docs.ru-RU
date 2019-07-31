---
title: Создание Андроидтрустедрутцертификате
description: Создание нового объекта Андроидтрустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c12d561af51d2badccc2d19e594566cd709ab1e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962640"
---
# <a name="create-androidtrustedrootcertificate"></a><span data-ttu-id="55705-103">Создание Андроидтрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="55705-103">Create androidTrustedRootCertificate</span></span>

> <span data-ttu-id="55705-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55705-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55705-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55705-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55705-106">Создание нового объекта [андроидтрустедрутцертификате](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="55705-106">Create a new [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55705-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55705-107">Prerequisites</span></span>
<span data-ttu-id="55705-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55705-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55705-110">Permission type</span></span>|<span data-ttu-id="55705-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55705-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55705-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55705-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55705-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55705-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55705-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55705-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55705-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55705-115">Not supported.</span></span>|
|<span data-ttu-id="55705-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55705-116">Application</span></span>|<span data-ttu-id="55705-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55705-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55705-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55705-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="55705-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55705-119">Request headers</span></span>
|<span data-ttu-id="55705-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55705-120">Header</span></span>|<span data-ttu-id="55705-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55705-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55705-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55705-122">Authorization</span></span>|<span data-ttu-id="55705-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55705-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55705-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55705-124">Accept</span></span>|<span data-ttu-id="55705-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55705-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55705-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55705-126">Request body</span></span>
<span data-ttu-id="55705-127">В тексте запроса добавьте представление объекта Андроидтрустедрутцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55705-127">In the request body, supply a JSON representation for the androidTrustedRootCertificate object.</span></span>

<span data-ttu-id="55705-128">В следующей таблице приведены свойства, необходимые при создании Андроидтрустедрутцертификате.</span><span class="sxs-lookup"><span data-stu-id="55705-128">The following table shows the properties that are required when you create the androidTrustedRootCertificate.</span></span>

|<span data-ttu-id="55705-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55705-129">Property</span></span>|<span data-ttu-id="55705-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55705-130">Type</span></span>|<span data-ttu-id="55705-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55705-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55705-132">id</span><span class="sxs-lookup"><span data-stu-id="55705-132">id</span></span>|<span data-ttu-id="55705-133">String</span><span class="sxs-lookup"><span data-stu-id="55705-133">String</span></span>|<span data-ttu-id="55705-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55705-134">Key of the entity.</span></span> <span data-ttu-id="55705-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55705-136">lastModifiedDateTime</span></span>|<span data-ttu-id="55705-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55705-137">DateTimeOffset</span></span>|<span data-ttu-id="55705-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="55705-138">DateTime the object was last modified.</span></span> <span data-ttu-id="55705-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="55705-140">roleScopeTagIds</span></span>|<span data-ttu-id="55705-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="55705-141">String collection</span></span>|<span data-ttu-id="55705-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="55705-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="55705-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="55705-144">supportsScopeTags</span></span>|<span data-ttu-id="55705-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="55705-145">Boolean</span></span>|<span data-ttu-id="55705-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="55705-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="55705-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="55705-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="55705-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="55705-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="55705-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55705-149">This property is read-only.</span></span> <span data-ttu-id="55705-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="55705-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="55705-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="55705-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="55705-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55705-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="55705-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="55705-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="55705-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="55705-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="55705-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55705-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="55705-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="55705-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="55705-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="55705-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="55705-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55705-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="55705-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55705-163">createdDateTime</span></span>|<span data-ttu-id="55705-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55705-164">DateTimeOffset</span></span>|<span data-ttu-id="55705-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="55705-165">DateTime the object was created.</span></span> <span data-ttu-id="55705-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-167">description</span><span class="sxs-lookup"><span data-stu-id="55705-167">description</span></span>|<span data-ttu-id="55705-168">String</span><span class="sxs-lookup"><span data-stu-id="55705-168">String</span></span>|<span data-ttu-id="55705-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55705-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55705-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-171">displayName</span><span class="sxs-lookup"><span data-stu-id="55705-171">displayName</span></span>|<span data-ttu-id="55705-172">Строка</span><span class="sxs-lookup"><span data-stu-id="55705-172">String</span></span>|<span data-ttu-id="55705-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55705-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55705-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-175">version</span><span class="sxs-lookup"><span data-stu-id="55705-175">version</span></span>|<span data-ttu-id="55705-176">Int32</span><span class="sxs-lookup"><span data-stu-id="55705-176">Int32</span></span>|<span data-ttu-id="55705-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55705-177">Version of the device configuration.</span></span> <span data-ttu-id="55705-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55705-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55705-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55705-179">trustedRootCertificate</span></span>|<span data-ttu-id="55705-180">Binary</span><span class="sxs-lookup"><span data-stu-id="55705-180">Binary</span></span>|<span data-ttu-id="55705-181">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="55705-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="55705-182">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="55705-182">certFileName</span></span>|<span data-ttu-id="55705-183">String</span><span class="sxs-lookup"><span data-stu-id="55705-183">String</span></span>|<span data-ttu-id="55705-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="55705-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="55705-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="55705-185">Response</span></span>
<span data-ttu-id="55705-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидтрустедрутцертификате](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55705-186">If successful, this method returns a `201 Created` response code and a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55705-187">Пример</span><span class="sxs-lookup"><span data-stu-id="55705-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="55705-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="55705-188">Request</span></span>
<span data-ttu-id="55705-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55705-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="55705-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="55705-190">Response</span></span>
<span data-ttu-id="55705-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55705-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1312

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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





