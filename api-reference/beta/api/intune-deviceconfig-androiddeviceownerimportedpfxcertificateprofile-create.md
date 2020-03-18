---
title: Создание Андроиддевицеовнеримпортедпфксцертификатепрофиле
description: Создание нового объекта Андроиддевицеовнеримпортедпфксцертификатепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bb2dfaf4410ac7e3bb1973dba74c348880033d6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759789"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="888ac-103">Создание Андроиддевицеовнеримпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="888ac-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="888ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="888ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="888ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="888ac-106">Создание нового объекта [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="888ac-106">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="888ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="888ac-107">Prerequisites</span></span>
<span data-ttu-id="888ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="888ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="888ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="888ac-110">Permission type</span></span>|<span data-ttu-id="888ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="888ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="888ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="888ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="888ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="888ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="888ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="888ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="888ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888ac-115">Not supported.</span></span>|
|<span data-ttu-id="888ac-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="888ac-116">Application</span></span>|<span data-ttu-id="888ac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="888ac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="888ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="888ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="888ac-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="888ac-119">Request headers</span></span>
|<span data-ttu-id="888ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="888ac-120">Header</span></span>|<span data-ttu-id="888ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="888ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="888ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="888ac-122">Authorization</span></span>|<span data-ttu-id="888ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="888ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="888ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="888ac-124">Accept</span></span>|<span data-ttu-id="888ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="888ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="888ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="888ac-126">Request body</span></span>
<span data-ttu-id="888ac-127">В тексте запроса добавьте представление объекта Андроиддевицеовнеримпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="888ac-127">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="888ac-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеримпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="888ac-128">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="888ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="888ac-129">Property</span></span>|<span data-ttu-id="888ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="888ac-130">Type</span></span>|<span data-ttu-id="888ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="888ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="888ac-132">id</span><span class="sxs-lookup"><span data-stu-id="888ac-132">id</span></span>|<span data-ttu-id="888ac-133">String</span><span class="sxs-lookup"><span data-stu-id="888ac-133">String</span></span>|<span data-ttu-id="888ac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="888ac-134">Key of the entity.</span></span> <span data-ttu-id="888ac-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="888ac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="888ac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="888ac-137">DateTimeOffset</span></span>|<span data-ttu-id="888ac-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="888ac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="888ac-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="888ac-140">roleScopeTagIds</span></span>|<span data-ttu-id="888ac-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="888ac-141">String collection</span></span>|<span data-ttu-id="888ac-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="888ac-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="888ac-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="888ac-144">supportsScopeTags</span></span>|<span data-ttu-id="888ac-145">Логический</span><span class="sxs-lookup"><span data-stu-id="888ac-145">Boolean</span></span>|<span data-ttu-id="888ac-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="888ac-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="888ac-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="888ac-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="888ac-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="888ac-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="888ac-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="888ac-149">This property is read-only.</span></span> <span data-ttu-id="888ac-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="888ac-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="888ac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="888ac-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="888ac-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="888ac-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="888ac-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="888ac-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="888ac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="888ac-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="888ac-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="888ac-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="888ac-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="888ac-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="888ac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="888ac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="888ac-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="888ac-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="888ac-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="888ac-163">createdDateTime</span></span>|<span data-ttu-id="888ac-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="888ac-164">DateTimeOffset</span></span>|<span data-ttu-id="888ac-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="888ac-165">DateTime the object was created.</span></span> <span data-ttu-id="888ac-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-167">description</span><span class="sxs-lookup"><span data-stu-id="888ac-167">description</span></span>|<span data-ttu-id="888ac-168">String</span><span class="sxs-lookup"><span data-stu-id="888ac-168">String</span></span>|<span data-ttu-id="888ac-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="888ac-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="888ac-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-171">displayName</span><span class="sxs-lookup"><span data-stu-id="888ac-171">displayName</span></span>|<span data-ttu-id="888ac-172">Строка</span><span class="sxs-lookup"><span data-stu-id="888ac-172">String</span></span>|<span data-ttu-id="888ac-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="888ac-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="888ac-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-175">version</span><span class="sxs-lookup"><span data-stu-id="888ac-175">version</span></span>|<span data-ttu-id="888ac-176">Int32</span><span class="sxs-lookup"><span data-stu-id="888ac-176">Int32</span></span>|<span data-ttu-id="888ac-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="888ac-177">Version of the device configuration.</span></span> <span data-ttu-id="888ac-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="888ac-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="888ac-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="888ac-180">Int32</span><span class="sxs-lookup"><span data-stu-id="888ac-180">Int32</span></span>|<span data-ttu-id="888ac-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="888ac-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="888ac-182">Допустимые значения — от 1 до 99, наследуемые от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="888ac-182">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="888ac-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="888ac-183">subjectNameFormat</span></span>|[<span data-ttu-id="888ac-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="888ac-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="888ac-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="888ac-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="888ac-186">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-186">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="888ac-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="888ac-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="888ac-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="888ac-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="888ac-189">Int32</span><span class="sxs-lookup"><span data-stu-id="888ac-189">Int32</span></span>|<span data-ttu-id="888ac-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="888ac-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="888ac-191">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="888ac-191">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="888ac-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="888ac-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="888ac-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="888ac-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="888ac-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="888ac-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="888ac-195">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-195">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="888ac-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="888ac-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="888ac-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="888ac-197">extendedKeyUsages</span></span>|<span data-ttu-id="888ac-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="888ac-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="888ac-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="888ac-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="888ac-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="888ac-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="888ac-201">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="888ac-201">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="888ac-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="888ac-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="888ac-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="888ac-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="888ac-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="888ac-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="888ac-205">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="888ac-205">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="888ac-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="888ac-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="888ac-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="888ac-207">intendedPurpose</span></span>|[<span data-ttu-id="888ac-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="888ac-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="888ac-209">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="888ac-209">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="888ac-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="888ac-210">Response</span></span>
<span data-ttu-id="888ac-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="888ac-211">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="888ac-212">Пример</span><span class="sxs-lookup"><span data-stu-id="888ac-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="888ac-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="888ac-213">Request</span></span>
<span data-ttu-id="888ac-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="888ac-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1503

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="888ac-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="888ac-215">Response</span></span>
<span data-ttu-id="888ac-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="888ac-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1675

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
  "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
  "intendedPurpose": "smimeEncryption"
}
```




