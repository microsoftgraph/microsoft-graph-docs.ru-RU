---
title: Обновление Андроидворкпрофилепкксцертификатепрофиле
description: Обновление свойств объекта Андроидворкпрофилепкксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 310121f115e7e2f4f3c72c7a4ca1b8b73a0ad9ba
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175773"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="e2f12-103">Обновление Андроидворкпрофилепкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="e2f12-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="e2f12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2f12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2f12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2f12-106">Обновление свойств объекта [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e2f12-106">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2f12-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2f12-107">Prerequisites</span></span>
<span data-ttu-id="e2f12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2f12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f12-110">Permission type</span></span>|<span data-ttu-id="e2f12-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2f12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2f12-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2f12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2f12-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f12-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2f12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2f12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f12-115">Not supported.</span></span>|
|<span data-ttu-id="e2f12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2f12-116">Application</span></span>|<span data-ttu-id="e2f12-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f12-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2f12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e2f12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2f12-119">Request headers</span></span>
|<span data-ttu-id="e2f12-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2f12-120">Header</span></span>|<span data-ttu-id="e2f12-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e2f12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2f12-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2f12-122">Authorization</span></span>|<span data-ttu-id="e2f12-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2f12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2f12-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2f12-124">Accept</span></span>|<span data-ttu-id="e2f12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2f12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f12-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2f12-126">Request body</span></span>
<span data-ttu-id="e2f12-127">В тексте запроса добавьте представление объекта [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2f12-127">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="e2f12-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-128">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="e2f12-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2f12-129">Property</span></span>|<span data-ttu-id="e2f12-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e2f12-130">Type</span></span>|<span data-ttu-id="e2f12-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f12-132">id</span><span class="sxs-lookup"><span data-stu-id="e2f12-132">id</span></span>|<span data-ttu-id="e2f12-133">String</span><span class="sxs-lookup"><span data-stu-id="e2f12-133">String</span></span>|<span data-ttu-id="e2f12-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2f12-134">Key of the entity.</span></span> <span data-ttu-id="e2f12-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f12-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e2f12-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f12-137">DateTimeOffset</span></span>|<span data-ttu-id="e2f12-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2f12-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e2f12-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2f12-140">roleScopeTagIds</span></span>|<span data-ttu-id="e2f12-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e2f12-141">String collection</span></span>|<span data-ttu-id="e2f12-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e2f12-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2f12-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e2f12-144">supportsScopeTags</span></span>|<span data-ttu-id="e2f12-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e2f12-145">Boolean</span></span>|<span data-ttu-id="e2f12-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e2f12-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2f12-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e2f12-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2f12-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e2f12-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2f12-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2f12-149">This property is read-only.</span></span> <span data-ttu-id="e2f12-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2f12-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2f12-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2f12-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2f12-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2f12-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2f12-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2f12-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2f12-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2f12-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2f12-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2f12-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2f12-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e2f12-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2f12-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e2f12-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2f12-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2f12-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2f12-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f12-163">createdDateTime</span></span>|<span data-ttu-id="e2f12-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f12-164">DateTimeOffset</span></span>|<span data-ttu-id="e2f12-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2f12-165">DateTime the object was created.</span></span> <span data-ttu-id="e2f12-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-167">description</span><span class="sxs-lookup"><span data-stu-id="e2f12-167">description</span></span>|<span data-ttu-id="e2f12-168">String</span><span class="sxs-lookup"><span data-stu-id="e2f12-168">String</span></span>|<span data-ttu-id="e2f12-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2f12-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2f12-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e2f12-171">displayName</span></span>|<span data-ttu-id="e2f12-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f12-172">String</span></span>|<span data-ttu-id="e2f12-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2f12-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2f12-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-175">version</span><span class="sxs-lookup"><span data-stu-id="e2f12-175">version</span></span>|<span data-ttu-id="e2f12-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f12-176">Int32</span></span>|<span data-ttu-id="e2f12-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2f12-177">Version of the device configuration.</span></span> <span data-ttu-id="e2f12-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2f12-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="e2f12-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="e2f12-180">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f12-180">Int32</span></span>|<span data-ttu-id="e2f12-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="e2f12-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e2f12-182">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e2f12-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e2f12-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e2f12-183">subjectNameFormat</span></span>|[<span data-ttu-id="e2f12-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e2f12-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e2f12-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e2f12-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="e2f12-186">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="e2f12-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e2f12-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e2f12-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e2f12-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e2f12-189">Int32</span><span class="sxs-lookup"><span data-stu-id="e2f12-189">Int32</span></span>|<span data-ttu-id="e2f12-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e2f12-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="e2f12-191">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e2f12-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e2f12-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e2f12-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e2f12-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e2f12-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e2f12-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e2f12-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e2f12-195">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="e2f12-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e2f12-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e2f12-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="e2f12-197">extendedKeyUsages</span></span>|<span data-ttu-id="e2f12-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="e2f12-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e2f12-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="e2f12-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e2f12-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2f12-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e2f12-201">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e2f12-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e2f12-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e2f12-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e2f12-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e2f12-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e2f12-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e2f12-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e2f12-205">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e2f12-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="e2f12-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e2f12-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e2f12-207">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="e2f12-207">certificationAuthority</span></span>|<span data-ttu-id="e2f12-208">String.</span><span class="sxs-lookup"><span data-stu-id="e2f12-208">String</span></span>|<span data-ttu-id="e2f12-209">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="e2f12-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="e2f12-210">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="e2f12-210">certificationAuthorityName</span></span>|<span data-ttu-id="e2f12-211">String.</span><span class="sxs-lookup"><span data-stu-id="e2f12-211">String</span></span>|<span data-ttu-id="e2f12-212">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="e2f12-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="e2f12-213">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="e2f12-213">certificateTemplateName</span></span>|<span data-ttu-id="e2f12-214">String.</span><span class="sxs-lookup"><span data-stu-id="e2f12-214">String</span></span>|<span data-ttu-id="e2f12-215">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="e2f12-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="e2f12-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e2f12-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e2f12-217">String.</span><span class="sxs-lookup"><span data-stu-id="e2f12-217">String</span></span>|<span data-ttu-id="e2f12-218">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="e2f12-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="e2f12-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f12-219">Response</span></span>
<span data-ttu-id="e2f12-220">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2f12-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2f12-221">Пример</span><span class="sxs-lookup"><span data-stu-id="e2f12-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2f12-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2f12-222">Request</span></span>
<span data-ttu-id="e2f12-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2f12-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1742

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="e2f12-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f12-224">Response</span></span>
<span data-ttu-id="e2f12-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2f12-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1914

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




