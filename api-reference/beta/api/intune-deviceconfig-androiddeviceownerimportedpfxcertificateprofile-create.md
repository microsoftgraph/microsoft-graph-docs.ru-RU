---
title: Создание Андроиддевицеовнеримпортедпфксцертификатепрофиле
description: Создание нового объекта Андроиддевицеовнеримпортедпфксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc6bc63cd5117028cb4b421319a4c08996959011
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436227"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="ccca2-103">Создание Андроиддевицеовнеримпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="ccca2-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="ccca2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccca2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccca2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccca2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccca2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccca2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccca2-107">Создание нового объекта [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ccca2-107">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccca2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccca2-108">Prerequisites</span></span>
<span data-ttu-id="ccca2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccca2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccca2-111">Permission type</span></span>|<span data-ttu-id="ccca2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccca2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccca2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccca2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccca2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccca2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccca2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccca2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccca2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccca2-116">Not supported.</span></span>|
|<span data-ttu-id="ccca2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ccca2-117">Application</span></span>|<span data-ttu-id="ccca2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccca2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccca2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccca2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ccca2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccca2-120">Request headers</span></span>
|<span data-ttu-id="ccca2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccca2-121">Header</span></span>|<span data-ttu-id="ccca2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ccca2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccca2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccca2-123">Authorization</span></span>|<span data-ttu-id="ccca2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccca2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccca2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ccca2-125">Accept</span></span>|<span data-ttu-id="ccca2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccca2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccca2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccca2-127">Request body</span></span>
<span data-ttu-id="ccca2-128">В тексте запроса добавьте представление объекта Андроиддевицеовнеримпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccca2-128">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="ccca2-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеримпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="ccca2-129">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="ccca2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccca2-130">Property</span></span>|<span data-ttu-id="ccca2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ccca2-131">Type</span></span>|<span data-ttu-id="ccca2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccca2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccca2-133">id</span><span class="sxs-lookup"><span data-stu-id="ccca2-133">id</span></span>|<span data-ttu-id="ccca2-134">String</span><span class="sxs-lookup"><span data-stu-id="ccca2-134">String</span></span>|<span data-ttu-id="ccca2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ccca2-135">Key of the entity.</span></span> <span data-ttu-id="ccca2-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccca2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ccca2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccca2-138">DateTimeOffset</span></span>|<span data-ttu-id="ccca2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ccca2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ccca2-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ccca2-141">roleScopeTagIds</span></span>|<span data-ttu-id="ccca2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ccca2-142">String collection</span></span>|<span data-ttu-id="ccca2-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ccca2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ccca2-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ccca2-145">supportsScopeTags</span></span>|<span data-ttu-id="ccca2-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="ccca2-146">Boolean</span></span>|<span data-ttu-id="ccca2-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ccca2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ccca2-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ccca2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ccca2-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ccca2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ccca2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccca2-150">This property is read-only.</span></span> <span data-ttu-id="ccca2-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ccca2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ccca2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ccca2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ccca2-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ccca2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ccca2-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ccca2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ccca2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ccca2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ccca2-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ccca2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ccca2-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ccca2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ccca2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ccca2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ccca2-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ccca2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ccca2-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccca2-164">createdDateTime</span></span>|<span data-ttu-id="ccca2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccca2-165">DateTimeOffset</span></span>|<span data-ttu-id="ccca2-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ccca2-166">DateTime the object was created.</span></span> <span data-ttu-id="ccca2-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-168">description</span><span class="sxs-lookup"><span data-stu-id="ccca2-168">description</span></span>|<span data-ttu-id="ccca2-169">String</span><span class="sxs-lookup"><span data-stu-id="ccca2-169">String</span></span>|<span data-ttu-id="ccca2-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccca2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ccca2-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ccca2-172">displayName</span></span>|<span data-ttu-id="ccca2-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ccca2-173">String</span></span>|<span data-ttu-id="ccca2-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccca2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ccca2-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-176">version</span><span class="sxs-lookup"><span data-stu-id="ccca2-176">version</span></span>|<span data-ttu-id="ccca2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ccca2-177">Int32</span></span>|<span data-ttu-id="ccca2-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccca2-178">Version of the device configuration.</span></span> <span data-ttu-id="ccca2-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccca2-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="ccca2-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="ccca2-181">Int32</span><span class="sxs-lookup"><span data-stu-id="ccca2-181">Int32</span></span>|<span data-ttu-id="ccca2-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccca2-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ccca2-183">Допустимые значения — от 1 до 99, наследуемые от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ccca2-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ccca2-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ccca2-184">subjectNameFormat</span></span>|[<span data-ttu-id="ccca2-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ccca2-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ccca2-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccca2-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="ccca2-187">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="ccca2-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="ccca2-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ccca2-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ccca2-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ccca2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="ccca2-190">Int32</span></span>|<span data-ttu-id="ccca2-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccca2-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ccca2-192">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ccca2-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ccca2-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ccca2-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ccca2-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ccca2-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ccca2-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccca2-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ccca2-196">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="ccca2-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ccca2-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ccca2-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="ccca2-198">extendedKeyUsages</span></span>|<span data-ttu-id="ccca2-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="ccca2-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ccca2-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="ccca2-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ccca2-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ccca2-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ccca2-202">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ccca2-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ccca2-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ccca2-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ccca2-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ccca2-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ccca2-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccca2-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ccca2-206">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccca2-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="ccca2-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ccca2-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ccca2-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ccca2-208">intendedPurpose</span></span>|[<span data-ttu-id="ccca2-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ccca2-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="ccca2-210">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="ccca2-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="ccca2-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccca2-211">Response</span></span>
<span data-ttu-id="ccca2-212">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccca2-212">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccca2-213">Пример</span><span class="sxs-lookup"><span data-stu-id="ccca2-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccca2-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccca2-214">Request</span></span>
<span data-ttu-id="ccca2-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccca2-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ccca2-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccca2-216">Response</span></span>
<span data-ttu-id="ccca2-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccca2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



