---
title: Создание Иоседудевицеконфигуратион
description: Создание нового объекта Иоседудевицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70f053dd57f7e6b232efa85e28227eec3de2b6f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448958"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="c94a8-103">Создание Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c94a8-103">Create iosEduDeviceConfiguration</span></span>

<span data-ttu-id="c94a8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c94a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c94a8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c94a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c94a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c94a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c94a8-107">Создание нового объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c94a8-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c94a8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c94a8-108">Prerequisites</span></span>
<span data-ttu-id="c94a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c94a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c94a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c94a8-111">Permission type</span></span>|<span data-ttu-id="c94a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c94a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c94a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c94a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c94a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c94a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c94a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c94a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c94a8-116">Not supported.</span></span>|
|<span data-ttu-id="c94a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c94a8-117">Application</span></span>|<span data-ttu-id="c94a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c94a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c94a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c94a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c94a8-120">Request headers</span></span>
|<span data-ttu-id="c94a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c94a8-121">Header</span></span>|<span data-ttu-id="c94a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c94a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c94a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c94a8-123">Authorization</span></span>|<span data-ttu-id="c94a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c94a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c94a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c94a8-125">Accept</span></span>|<span data-ttu-id="c94a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c94a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c94a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c94a8-127">Request body</span></span>
<span data-ttu-id="c94a8-128">В тексте запроса добавьте представление объекта Иоседудевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c94a8-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="c94a8-129">В следующей таблице приведены свойства, необходимые при создании Иоседудевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="c94a8-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="c94a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c94a8-130">Property</span></span>|<span data-ttu-id="c94a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c94a8-131">Type</span></span>|<span data-ttu-id="c94a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c94a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94a8-133">id</span><span class="sxs-lookup"><span data-stu-id="c94a8-133">id</span></span>|<span data-ttu-id="c94a8-134">String</span><span class="sxs-lookup"><span data-stu-id="c94a8-134">String</span></span>|<span data-ttu-id="c94a8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c94a8-135">Key of the entity.</span></span> <span data-ttu-id="c94a8-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c94a8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c94a8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94a8-138">DateTimeOffset</span></span>|<span data-ttu-id="c94a8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c94a8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c94a8-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c94a8-141">roleScopeTagIds</span></span>|<span data-ttu-id="c94a8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c94a8-142">String collection</span></span>|<span data-ttu-id="c94a8-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c94a8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c94a8-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c94a8-145">supportsScopeTags</span></span>|<span data-ttu-id="c94a8-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c94a8-146">Boolean</span></span>|<span data-ttu-id="c94a8-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c94a8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c94a8-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c94a8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c94a8-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c94a8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c94a8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c94a8-150">This property is read-only.</span></span> <span data-ttu-id="c94a8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94a8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c94a8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94a8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c94a8-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c94a8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c94a8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94a8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c94a8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94a8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c94a8-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c94a8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c94a8-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94a8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c94a8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94a8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c94a8-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c94a8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c94a8-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c94a8-164">createdDateTime</span></span>|<span data-ttu-id="c94a8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94a8-165">DateTimeOffset</span></span>|<span data-ttu-id="c94a8-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c94a8-166">DateTime the object was created.</span></span> <span data-ttu-id="c94a8-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-168">description</span><span class="sxs-lookup"><span data-stu-id="c94a8-168">description</span></span>|<span data-ttu-id="c94a8-169">String</span><span class="sxs-lookup"><span data-stu-id="c94a8-169">String</span></span>|<span data-ttu-id="c94a8-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c94a8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c94a8-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c94a8-172">displayName</span></span>|<span data-ttu-id="c94a8-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c94a8-173">String</span></span>|<span data-ttu-id="c94a8-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c94a8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c94a8-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-176">version</span><span class="sxs-lookup"><span data-stu-id="c94a8-176">version</span></span>|<span data-ttu-id="c94a8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c94a8-177">Int32</span></span>|<span data-ttu-id="c94a8-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c94a8-178">Version of the device configuration.</span></span> <span data-ttu-id="c94a8-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c94a8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94a8-180">теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="c94a8-180">teacherCertificateSettings</span></span>|<span data-ttu-id="c94a8-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="c94a8-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="c94a8-182">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="c94a8-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="c94a8-183">студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="c94a8-183">studentCertificateSettings</span></span>|<span data-ttu-id="c94a8-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="c94a8-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="c94a8-185">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="c94a8-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="c94a8-186">девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="c94a8-186">deviceCertificateSettings</span></span>|<span data-ttu-id="c94a8-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="c94a8-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="c94a8-188">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="c94a8-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="c94a8-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="c94a8-189">Response</span></span>
<span data-ttu-id="c94a8-190">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c94a8-190">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c94a8-191">Пример</span><span class="sxs-lookup"><span data-stu-id="c94a8-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="c94a8-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="c94a8-192">Request</span></span>
<span data-ttu-id="c94a8-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c94a8-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c94a8-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="c94a8-194">Response</span></span>
<span data-ttu-id="c94a8-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c94a8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





