---
title: Создание Иоседудевицеконфигуратион
description: Создание нового объекта Иоседудевицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd58a1c0c765a38b8c19364ff0d33d7ce139e5e0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167742"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="9b762-103">Создание Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b762-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="9b762-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b762-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b762-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b762-106">Создание нового объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b762-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b762-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b762-107">Prerequisites</span></span>
<span data-ttu-id="9b762-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b762-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b762-110">Permission type</span></span>|<span data-ttu-id="9b762-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b762-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b762-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b762-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b762-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b762-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b762-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b762-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b762-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b762-115">Not supported.</span></span>|
|<span data-ttu-id="9b762-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b762-116">Application</span></span>|<span data-ttu-id="9b762-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b762-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b762-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b762-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9b762-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b762-119">Request headers</span></span>
|<span data-ttu-id="9b762-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b762-120">Header</span></span>|<span data-ttu-id="9b762-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b762-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b762-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b762-122">Authorization</span></span>|<span data-ttu-id="9b762-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b762-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b762-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b762-124">Accept</span></span>|<span data-ttu-id="9b762-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b762-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b762-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b762-126">Request body</span></span>
<span data-ttu-id="9b762-127">В тексте запроса добавьте представление объекта Иоседудевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b762-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="9b762-128">В следующей таблице приведены свойства, необходимые при создании Иоседудевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="9b762-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="9b762-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b762-129">Property</span></span>|<span data-ttu-id="9b762-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9b762-130">Type</span></span>|<span data-ttu-id="9b762-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9b762-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b762-132">id</span><span class="sxs-lookup"><span data-stu-id="9b762-132">id</span></span>|<span data-ttu-id="9b762-133">String</span><span class="sxs-lookup"><span data-stu-id="9b762-133">String</span></span>|<span data-ttu-id="9b762-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9b762-134">Key of the entity.</span></span> <span data-ttu-id="9b762-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b762-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9b762-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b762-137">DateTimeOffset</span></span>|<span data-ttu-id="9b762-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9b762-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9b762-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b762-140">roleScopeTagIds</span></span>|<span data-ttu-id="9b762-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9b762-141">String collection</span></span>|<span data-ttu-id="9b762-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9b762-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b762-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9b762-144">supportsScopeTags</span></span>|<span data-ttu-id="9b762-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9b762-145">Boolean</span></span>|<span data-ttu-id="9b762-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9b762-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b762-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9b762-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b762-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9b762-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b762-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b762-149">This property is read-only.</span></span> <span data-ttu-id="9b762-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b762-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9b762-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b762-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9b762-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b762-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9b762-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b762-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9b762-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b762-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9b762-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b762-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9b762-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9b762-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9b762-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9b762-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9b762-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b762-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9b762-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b762-163">createdDateTime</span></span>|<span data-ttu-id="9b762-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b762-164">DateTimeOffset</span></span>|<span data-ttu-id="9b762-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9b762-165">DateTime the object was created.</span></span> <span data-ttu-id="9b762-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-167">description</span><span class="sxs-lookup"><span data-stu-id="9b762-167">description</span></span>|<span data-ttu-id="9b762-168">String</span><span class="sxs-lookup"><span data-stu-id="9b762-168">String</span></span>|<span data-ttu-id="9b762-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b762-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b762-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9b762-171">displayName</span></span>|<span data-ttu-id="9b762-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9b762-172">String</span></span>|<span data-ttu-id="9b762-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b762-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b762-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-175">version</span><span class="sxs-lookup"><span data-stu-id="9b762-175">version</span></span>|<span data-ttu-id="9b762-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9b762-176">Int32</span></span>|<span data-ttu-id="9b762-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b762-177">Version of the device configuration.</span></span> <span data-ttu-id="9b762-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b762-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b762-179">теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="9b762-179">teacherCertificateSettings</span></span>|<span data-ttu-id="9b762-180">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="9b762-180">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="9b762-181">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="9b762-181">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="9b762-182">студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="9b762-182">studentCertificateSettings</span></span>|<span data-ttu-id="9b762-183">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="9b762-183">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="9b762-184">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="9b762-184">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="9b762-185">девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="9b762-185">deviceCertificateSettings</span></span>|<span data-ttu-id="9b762-186">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="9b762-186">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="9b762-187">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="9b762-187">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="9b762-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b762-188">Response</span></span>
<span data-ttu-id="9b762-189">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b762-189">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b762-190">Пример</span><span class="sxs-lookup"><span data-stu-id="9b762-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b762-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b762-191">Request</span></span>
<span data-ttu-id="9b762-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b762-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b762-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b762-193">Response</span></span>
<span data-ttu-id="9b762-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b762-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




