---
title: Обновление Андроиддевицеовнерсцепцертификатепрофиле
description: Обновление свойств объекта Андроиддевицеовнерсцепцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7572b205dc6e14a3269e5665fb2ba1adc0a133b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43350534"
---
# <a name="update-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="d2749-103">Обновление Андроиддевицеовнерсцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="d2749-103">Update androidDeviceOwnerScepCertificateProfile</span></span>

<span data-ttu-id="d2749-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2749-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2749-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2749-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2749-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2749-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2749-107">Обновление свойств объекта [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d2749-107">Update the properties of a [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2749-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2749-108">Prerequisites</span></span>
<span data-ttu-id="d2749-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2749-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2749-111">Permission type</span></span>|<span data-ttu-id="d2749-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2749-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2749-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2749-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2749-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2749-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2749-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2749-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2749-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2749-116">Not supported.</span></span>|
|<span data-ttu-id="d2749-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d2749-117">Application</span></span>|<span data-ttu-id="d2749-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2749-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2749-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2749-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d2749-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2749-120">Request headers</span></span>
|<span data-ttu-id="d2749-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2749-121">Header</span></span>|<span data-ttu-id="d2749-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2749-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2749-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2749-123">Authorization</span></span>|<span data-ttu-id="d2749-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2749-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2749-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2749-125">Accept</span></span>|<span data-ttu-id="d2749-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2749-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2749-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2749-127">Request body</span></span>
<span data-ttu-id="d2749-128">В тексте запроса добавьте представление объекта [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2749-128">In the request body, supply a JSON representation for the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d2749-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-129">The following table shows the properties that are required when you create the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span></span>

|<span data-ttu-id="d2749-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2749-130">Property</span></span>|<span data-ttu-id="d2749-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d2749-131">Type</span></span>|<span data-ttu-id="d2749-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d2749-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2749-133">id</span><span class="sxs-lookup"><span data-stu-id="d2749-133">id</span></span>|<span data-ttu-id="d2749-134">String</span><span class="sxs-lookup"><span data-stu-id="d2749-134">String</span></span>|<span data-ttu-id="d2749-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2749-135">Key of the entity.</span></span> <span data-ttu-id="d2749-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2749-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d2749-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2749-138">DateTimeOffset</span></span>|<span data-ttu-id="d2749-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d2749-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d2749-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2749-141">roleScopeTagIds</span></span>|<span data-ttu-id="d2749-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2749-142">String collection</span></span>|<span data-ttu-id="d2749-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d2749-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2749-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d2749-145">supportsScopeTags</span></span>|<span data-ttu-id="d2749-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="d2749-146">Boolean</span></span>|<span data-ttu-id="d2749-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d2749-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2749-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d2749-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2749-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d2749-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2749-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2749-150">This property is read-only.</span></span> <span data-ttu-id="d2749-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2749-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d2749-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2749-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d2749-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d2749-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d2749-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2749-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d2749-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2749-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d2749-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d2749-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d2749-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d2749-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d2749-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d2749-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d2749-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d2749-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d2749-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2749-164">createdDateTime</span></span>|<span data-ttu-id="d2749-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2749-165">DateTimeOffset</span></span>|<span data-ttu-id="d2749-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d2749-166">DateTime the object was created.</span></span> <span data-ttu-id="d2749-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-168">description</span><span class="sxs-lookup"><span data-stu-id="d2749-168">description</span></span>|<span data-ttu-id="d2749-169">String</span><span class="sxs-lookup"><span data-stu-id="d2749-169">String</span></span>|<span data-ttu-id="d2749-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2749-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2749-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d2749-172">displayName</span></span>|<span data-ttu-id="d2749-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d2749-173">String</span></span>|<span data-ttu-id="d2749-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2749-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2749-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-176">version</span><span class="sxs-lookup"><span data-stu-id="d2749-176">version</span></span>|<span data-ttu-id="d2749-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d2749-177">Int32</span></span>|<span data-ttu-id="d2749-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2749-178">Version of the device configuration.</span></span> <span data-ttu-id="d2749-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2749-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="d2749-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="d2749-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d2749-181">Int32</span></span>|<span data-ttu-id="d2749-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2749-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d2749-183">Допустимые значения — от 1 до 99, наследуемые от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d2749-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2749-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d2749-184">subjectNameFormat</span></span>|[<span data-ttu-id="d2749-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d2749-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d2749-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2749-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="d2749-187">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d2749-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d2749-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d2749-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d2749-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d2749-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d2749-190">Int32</span></span>|<span data-ttu-id="d2749-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2749-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d2749-192">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d2749-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2749-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2749-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d2749-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2749-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d2749-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2749-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d2749-196">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d2749-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d2749-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d2749-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="d2749-198">extendedKeyUsages</span></span>|<span data-ttu-id="d2749-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d2749-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d2749-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="d2749-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d2749-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d2749-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d2749-202">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d2749-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2749-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d2749-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d2749-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d2749-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d2749-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2749-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d2749-206">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d2749-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d2749-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d2749-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d2749-208">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="d2749-208">scepServerUrls</span></span>|<span data-ttu-id="d2749-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2749-209">String collection</span></span>|<span data-ttu-id="d2749-210">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="d2749-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="d2749-211">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="d2749-211">subjectNameFormatString</span></span>|<span data-ttu-id="d2749-212">String</span><span class="sxs-lookup"><span data-stu-id="d2749-212">String</span></span>|<span data-ttu-id="d2749-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="d2749-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d2749-214">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="d2749-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d2749-215">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="d2749-215">keyUsage</span></span>|[<span data-ttu-id="d2749-216">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="d2749-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d2749-217">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="d2749-217">SCEP Key Usage.</span></span> <span data-ttu-id="d2749-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="d2749-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d2749-219">keySize</span><span class="sxs-lookup"><span data-stu-id="d2749-219">keySize</span></span>|[<span data-ttu-id="d2749-220">keySize</span><span class="sxs-lookup"><span data-stu-id="d2749-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d2749-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="d2749-221">SCEP Key Size.</span></span> <span data-ttu-id="d2749-222">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="d2749-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d2749-223">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="d2749-223">hashAlgorithm</span></span>|[<span data-ttu-id="d2749-224">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="d2749-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="d2749-225">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="d2749-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d2749-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="d2749-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d2749-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d2749-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d2749-228">String</span><span class="sxs-lookup"><span data-stu-id="d2749-228">String</span></span>|<span data-ttu-id="d2749-229">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="d2749-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d2749-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d2749-230">certificateStore</span></span>|[<span data-ttu-id="d2749-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d2749-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="d2749-232">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="d2749-232">Target store certificate.</span></span> <span data-ttu-id="d2749-233">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="d2749-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="d2749-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="d2749-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="d2749-235">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="d2749-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="d2749-236">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="d2749-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="d2749-237">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d2749-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d2749-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2749-238">Response</span></span>
<span data-ttu-id="d2749-239">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2749-239">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2749-240">Пример</span><span class="sxs-lookup"><span data-stu-id="d2749-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2749-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2749-241">Request</span></span>
<span data-ttu-id="d2749-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2749-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d2749-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2749-243">Response</span></span>
<span data-ttu-id="d2749-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2749-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```



