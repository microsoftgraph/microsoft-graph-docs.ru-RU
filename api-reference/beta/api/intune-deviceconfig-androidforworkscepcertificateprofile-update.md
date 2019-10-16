---
title: Обновление androidForWorkScepCertificateProfile
description: Обновление свойств объекта androidForWorkScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 483b7f671cfb540bd341d3972795fb90c491fed1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534549"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="0e834-103">Обновление androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0e834-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="0e834-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e834-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e834-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e834-106">Обновление свойств объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0e834-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e834-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e834-107">Prerequisites</span></span>
<span data-ttu-id="0e834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e834-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e834-110">Permission type</span></span>|<span data-ttu-id="0e834-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e834-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e834-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e834-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e834-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e834-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e834-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e834-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e834-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e834-115">Not supported.</span></span>|
|<span data-ttu-id="0e834-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e834-116">Application</span></span>|<span data-ttu-id="0e834-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e834-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e834-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e834-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e834-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e834-119">Request headers</span></span>
|<span data-ttu-id="0e834-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e834-120">Header</span></span>|<span data-ttu-id="0e834-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e834-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e834-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e834-122">Authorization</span></span>|<span data-ttu-id="0e834-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e834-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e834-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e834-124">Accept</span></span>|<span data-ttu-id="0e834-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e834-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e834-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e834-126">Request body</span></span>
<span data-ttu-id="0e834-127">В тексте запроса добавьте представление объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e834-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="0e834-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="0e834-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e834-129">Property</span></span>|<span data-ttu-id="0e834-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e834-130">Type</span></span>|<span data-ttu-id="0e834-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e834-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e834-132">id</span><span class="sxs-lookup"><span data-stu-id="0e834-132">id</span></span>|<span data-ttu-id="0e834-133">String</span><span class="sxs-lookup"><span data-stu-id="0e834-133">String</span></span>|<span data-ttu-id="0e834-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e834-134">Key of the entity.</span></span> <span data-ttu-id="0e834-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e834-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0e834-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e834-137">DateTimeOffset</span></span>|<span data-ttu-id="0e834-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0e834-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0e834-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e834-140">roleScopeTagIds</span></span>|<span data-ttu-id="0e834-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0e834-141">String collection</span></span>|<span data-ttu-id="0e834-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0e834-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e834-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0e834-144">supportsScopeTags</span></span>|<span data-ttu-id="0e834-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0e834-145">Boolean</span></span>|<span data-ttu-id="0e834-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0e834-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e834-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0e834-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e834-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0e834-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e834-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e834-149">This property is read-only.</span></span> <span data-ttu-id="0e834-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e834-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0e834-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e834-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0e834-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e834-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0e834-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e834-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0e834-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e834-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0e834-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e834-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0e834-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e834-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0e834-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e834-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0e834-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e834-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0e834-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e834-163">createdDateTime</span></span>|<span data-ttu-id="0e834-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e834-164">DateTimeOffset</span></span>|<span data-ttu-id="0e834-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0e834-165">DateTime the object was created.</span></span> <span data-ttu-id="0e834-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-167">description</span><span class="sxs-lookup"><span data-stu-id="0e834-167">description</span></span>|<span data-ttu-id="0e834-168">String</span><span class="sxs-lookup"><span data-stu-id="0e834-168">String</span></span>|<span data-ttu-id="0e834-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e834-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e834-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0e834-171">displayName</span></span>|<span data-ttu-id="0e834-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0e834-172">String</span></span>|<span data-ttu-id="0e834-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e834-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e834-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-175">version</span><span class="sxs-lookup"><span data-stu-id="0e834-175">version</span></span>|<span data-ttu-id="0e834-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0e834-176">Int32</span></span>|<span data-ttu-id="0e834-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e834-177">Version of the device configuration.</span></span> <span data-ttu-id="0e834-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e834-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="0e834-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="0e834-180">Int32</span><span class="sxs-lookup"><span data-stu-id="0e834-180">Int32</span></span>|<span data-ttu-id="0e834-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e834-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0e834-182">Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0e834-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0e834-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0e834-183">subjectNameFormat</span></span>|[<span data-ttu-id="0e834-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0e834-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0e834-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e834-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="0e834-186">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0e834-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="0e834-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0e834-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0e834-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0e834-189">Int32</span><span class="sxs-lookup"><span data-stu-id="0e834-189">Int32</span></span>|<span data-ttu-id="0e834-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e834-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0e834-191">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0e834-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0e834-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0e834-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0e834-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0e834-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0e834-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e834-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0e834-195">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0e834-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0e834-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0e834-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="0e834-197">extendedKeyUsages</span></span>|<span data-ttu-id="0e834-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="0e834-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0e834-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="0e834-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0e834-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e834-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0e834-201">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0e834-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0e834-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0e834-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0e834-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0e834-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0e834-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e834-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0e834-205">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0e834-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0e834-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0e834-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0e834-207">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="0e834-207">scepServerUrls</span></span>|<span data-ttu-id="0e834-208">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0e834-208">String collection</span></span>|<span data-ttu-id="0e834-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="0e834-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="0e834-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="0e834-210">subjectNameFormatString</span></span>|<span data-ttu-id="0e834-211">String</span><span class="sxs-lookup"><span data-stu-id="0e834-211">String</span></span>|<span data-ttu-id="0e834-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="0e834-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="0e834-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="0e834-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="0e834-214">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="0e834-214">keyUsage</span></span>|[<span data-ttu-id="0e834-215">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="0e834-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="0e834-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="0e834-216">SCEP Key Usage.</span></span> <span data-ttu-id="0e834-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="0e834-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="0e834-218">keySize</span><span class="sxs-lookup"><span data-stu-id="0e834-218">keySize</span></span>|[<span data-ttu-id="0e834-219">keySize</span><span class="sxs-lookup"><span data-stu-id="0e834-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="0e834-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="0e834-220">SCEP Key Size.</span></span> <span data-ttu-id="0e834-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="0e834-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="0e834-222">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="0e834-222">hashAlgorithm</span></span>|[<span data-ttu-id="0e834-223">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="0e834-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="0e834-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="0e834-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="0e834-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="0e834-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="0e834-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0e834-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0e834-227">String</span><span class="sxs-lookup"><span data-stu-id="0e834-227">String</span></span>|<span data-ttu-id="0e834-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="0e834-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="0e834-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0e834-229">certificateStore</span></span>|[<span data-ttu-id="0e834-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0e834-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="0e834-231">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="0e834-231">Target store certificate.</span></span> <span data-ttu-id="0e834-232">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0e834-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0e834-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="0e834-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="0e834-234">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="0e834-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0e834-235">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="0e834-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="0e834-236">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e834-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0e834-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e834-237">Response</span></span>
<span data-ttu-id="0e834-238">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e834-238">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e834-239">Пример</span><span class="sxs-lookup"><span data-stu-id="0e834-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e834-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e834-240">Request</span></span>
<span data-ttu-id="0e834-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e834-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1978

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="0e834-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e834-242">Response</span></span>
<span data-ttu-id="0e834-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e834-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2150

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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






