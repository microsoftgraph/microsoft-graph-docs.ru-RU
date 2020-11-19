---
title: Создание Иоседудевицеконфигуратион
description: Создание нового объекта Иоседудевицеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91220979f96e3a792e29755da75b11a597619de6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49264795"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="ee7f5-103">Создание Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ee7f5-103">Create iosEduDeviceConfiguration</span></span>

<span data-ttu-id="ee7f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee7f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee7f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee7f5-107">Создание нового объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee7f5-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee7f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee7f5-108">Prerequisites</span></span>
<span data-ttu-id="ee7f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee7f5-111">Permission type</span></span>|<span data-ttu-id="ee7f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee7f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee7f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee7f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee7f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee7f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee7f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-116">Not supported.</span></span>|
|<span data-ttu-id="ee7f5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ee7f5-117">Application</span></span>|<span data-ttu-id="ee7f5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7f5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee7f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ee7f5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee7f5-120">Request headers</span></span>
|<span data-ttu-id="ee7f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee7f5-121">Header</span></span>|<span data-ttu-id="ee7f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee7f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee7f5-123">Authorization</span></span>|<span data-ttu-id="ee7f5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee7f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee7f5-125">Accept</span></span>|<span data-ttu-id="ee7f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee7f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee7f5-127">Request body</span></span>
<span data-ttu-id="ee7f5-128">В тексте запроса добавьте представление объекта Иоседудевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="ee7f5-129">В следующей таблице приведены свойства, необходимые при создании Иоседудевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="ee7f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee7f5-130">Property</span></span>|<span data-ttu-id="ee7f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7f5-131">Type</span></span>|<span data-ttu-id="ee7f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee7f5-133">id</span><span class="sxs-lookup"><span data-stu-id="ee7f5-133">id</span></span>|<span data-ttu-id="ee7f5-134">String</span><span class="sxs-lookup"><span data-stu-id="ee7f5-134">String</span></span>|<span data-ttu-id="ee7f5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-135">Key of the entity.</span></span> <span data-ttu-id="ee7f5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ee7f5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f5-138">DateTimeOffset</span></span>|<span data-ttu-id="ee7f5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ee7f5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee7f5-141">roleScopeTagIds</span></span>|<span data-ttu-id="ee7f5-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ee7f5-142">String collection</span></span>|<span data-ttu-id="ee7f5-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee7f5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ee7f5-145">supportsScopeTags</span></span>|<span data-ttu-id="ee7f5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee7f5-146">Boolean</span></span>|<span data-ttu-id="ee7f5-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee7f5-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee7f5-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee7f5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-150">This property is read-only.</span></span> <span data-ttu-id="ee7f5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee7f5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ee7f5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee7f5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ee7f5-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ee7f5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee7f5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ee7f5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee7f5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ee7f5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ee7f5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ee7f5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ee7f5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ee7f5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ee7f5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ee7f5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f5-164">createdDateTime</span></span>|<span data-ttu-id="ee7f5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f5-165">DateTimeOffset</span></span>|<span data-ttu-id="ee7f5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-166">DateTime the object was created.</span></span> <span data-ttu-id="ee7f5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-168">description</span><span class="sxs-lookup"><span data-stu-id="ee7f5-168">description</span></span>|<span data-ttu-id="ee7f5-169">String</span><span class="sxs-lookup"><span data-stu-id="ee7f5-169">String</span></span>|<span data-ttu-id="ee7f5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee7f5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7f5-172">displayName</span></span>|<span data-ttu-id="ee7f5-173">String</span><span class="sxs-lookup"><span data-stu-id="ee7f5-173">String</span></span>|<span data-ttu-id="ee7f5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee7f5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-176">version</span><span class="sxs-lookup"><span data-stu-id="ee7f5-176">version</span></span>|<span data-ttu-id="ee7f5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7f5-177">Int32</span></span>|<span data-ttu-id="ee7f5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-178">Version of the device configuration.</span></span> <span data-ttu-id="ee7f5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f5-180">теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="ee7f5-180">teacherCertificateSettings</span></span>|<span data-ttu-id="ee7f5-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="ee7f5-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="ee7f5-182">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="ee7f5-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="ee7f5-183">студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="ee7f5-183">studentCertificateSettings</span></span>|<span data-ttu-id="ee7f5-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="ee7f5-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="ee7f5-185">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="ee7f5-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="ee7f5-186">девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="ee7f5-186">deviceCertificateSettings</span></span>|<span data-ttu-id="ee7f5-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="ee7f5-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="ee7f5-188">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="ee7f5-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="ee7f5-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee7f5-189">Response</span></span>
<span data-ttu-id="ee7f5-190">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-190">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7f5-191">Пример</span><span class="sxs-lookup"><span data-stu-id="ee7f5-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee7f5-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f5-192">Request</span></span>
<span data-ttu-id="ee7f5-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee7f5-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee7f5-194">Response</span></span>
<span data-ttu-id="ee7f5-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee7f5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




