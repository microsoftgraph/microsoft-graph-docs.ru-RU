---
title: Обновление Иоседудевицеконфигуратион
description: Обновление свойств объекта Иоседудевицеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2bcdc67b485c8d9cbcb02bfb532ec17c5d0af9d2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698899"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="d3e57-103">Обновление Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d3e57-103">Update iosEduDeviceConfiguration</span></span>

<span data-ttu-id="d3e57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3e57-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3e57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e57-107">Обновление свойств объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e57-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3e57-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3e57-108">Prerequisites</span></span>
<span data-ttu-id="d3e57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e57-111">Permission type</span></span>|<span data-ttu-id="d3e57-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3e57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3e57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3e57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3e57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3e57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3e57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e57-116">Not supported.</span></span>|
|<span data-ttu-id="d3e57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3e57-117">Application</span></span>|<span data-ttu-id="d3e57-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e57-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3e57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3e57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d3e57-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3e57-120">Request headers</span></span>
|<span data-ttu-id="d3e57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3e57-121">Header</span></span>|<span data-ttu-id="d3e57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3e57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3e57-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3e57-123">Authorization</span></span>|<span data-ttu-id="d3e57-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3e57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3e57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3e57-125">Accept</span></span>|<span data-ttu-id="d3e57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3e57-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3e57-127">Request body</span></span>
<span data-ttu-id="d3e57-128">В тексте запроса добавьте представление объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e57-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d3e57-129">В следующей таблице приведены свойства, необходимые при создании [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="d3e57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3e57-130">Property</span></span>|<span data-ttu-id="d3e57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3e57-131">Type</span></span>|<span data-ttu-id="d3e57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3e57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e57-133">id</span><span class="sxs-lookup"><span data-stu-id="d3e57-133">id</span></span>|<span data-ttu-id="d3e57-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d3e57-134">String</span></span>|<span data-ttu-id="d3e57-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d3e57-135">Key of the entity.</span></span> <span data-ttu-id="d3e57-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3e57-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d3e57-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e57-138">DateTimeOffset</span></span>|<span data-ttu-id="d3e57-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d3e57-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d3e57-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3e57-141">roleScopeTagIds</span></span>|<span data-ttu-id="d3e57-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d3e57-142">String collection</span></span>|<span data-ttu-id="d3e57-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d3e57-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d3e57-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d3e57-145">supportsScopeTags</span></span>|<span data-ttu-id="d3e57-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d3e57-146">Boolean</span></span>|<span data-ttu-id="d3e57-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d3e57-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d3e57-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d3e57-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d3e57-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d3e57-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d3e57-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3e57-150">This property is read-only.</span></span> <span data-ttu-id="d3e57-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3e57-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d3e57-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3e57-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d3e57-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3e57-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d3e57-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3e57-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d3e57-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3e57-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d3e57-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3e57-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d3e57-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3e57-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d3e57-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3e57-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d3e57-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3e57-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d3e57-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3e57-164">createdDateTime</span></span>|<span data-ttu-id="d3e57-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e57-165">DateTimeOffset</span></span>|<span data-ttu-id="d3e57-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d3e57-166">DateTime the object was created.</span></span> <span data-ttu-id="d3e57-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-168">description</span><span class="sxs-lookup"><span data-stu-id="d3e57-168">description</span></span>|<span data-ttu-id="d3e57-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d3e57-169">String</span></span>|<span data-ttu-id="d3e57-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3e57-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d3e57-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d3e57-172">displayName</span></span>|<span data-ttu-id="d3e57-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d3e57-173">String</span></span>|<span data-ttu-id="d3e57-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3e57-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d3e57-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-176">version</span><span class="sxs-lookup"><span data-stu-id="d3e57-176">version</span></span>|<span data-ttu-id="d3e57-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d3e57-177">Int32</span></span>|<span data-ttu-id="d3e57-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3e57-178">Version of the device configuration.</span></span> <span data-ttu-id="d3e57-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3e57-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3e57-180">теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="d3e57-180">teacherCertificateSettings</span></span>|<span data-ttu-id="d3e57-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d3e57-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d3e57-182">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="d3e57-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="d3e57-183">студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="d3e57-183">studentCertificateSettings</span></span>|<span data-ttu-id="d3e57-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d3e57-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d3e57-185">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="d3e57-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="d3e57-186">девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="d3e57-186">deviceCertificateSettings</span></span>|<span data-ttu-id="d3e57-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d3e57-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d3e57-188">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="d3e57-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="d3e57-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3e57-189">Response</span></span>
<span data-ttu-id="d3e57-190">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3e57-190">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e57-191">Пример</span><span class="sxs-lookup"><span data-stu-id="d3e57-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3e57-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3e57-192">Request</span></span>
<span data-ttu-id="d3e57-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3e57-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2683

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="d3e57-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e57-194">Response</span></span>
<span data-ttu-id="d3e57-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3e57-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2855

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





