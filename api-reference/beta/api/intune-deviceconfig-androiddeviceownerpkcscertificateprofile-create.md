---
title: Создание Андроиддевицеовнерпкксцертификатепрофиле
description: Создание нового объекта Андроиддевицеовнерпкксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7df03e38cbfb6abdc3691a1129714463bbd5cb14
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005889"
---
# <a name="create-androiddeviceownerpkcscertificateprofile"></a><span data-ttu-id="89289-103">Создание Андроиддевицеовнерпкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="89289-103">Create androidDeviceOwnerPkcsCertificateProfile</span></span>

<span data-ttu-id="89289-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89289-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89289-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89289-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89289-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89289-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89289-107">Создание нового объекта [андроиддевицеовнерпкксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="89289-107">Create a new [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89289-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89289-108">Prerequisites</span></span>
<span data-ttu-id="89289-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89289-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89289-111">Permission type</span></span>|<span data-ttu-id="89289-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89289-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89289-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89289-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89289-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89289-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89289-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89289-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89289-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89289-116">Not supported.</span></span>|
|<span data-ttu-id="89289-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="89289-117">Application</span></span>|<span data-ttu-id="89289-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89289-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89289-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89289-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89289-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89289-120">Request headers</span></span>
|<span data-ttu-id="89289-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89289-121">Header</span></span>|<span data-ttu-id="89289-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89289-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89289-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89289-123">Authorization</span></span>|<span data-ttu-id="89289-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89289-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89289-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89289-125">Accept</span></span>|<span data-ttu-id="89289-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89289-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89289-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89289-127">Request body</span></span>
<span data-ttu-id="89289-128">В тексте запроса добавьте представление объекта Андроиддевицеовнерпкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89289-128">In the request body, supply a JSON representation for the androidDeviceOwnerPkcsCertificateProfile object.</span></span>

<span data-ttu-id="89289-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерпкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="89289-129">The following table shows the properties that are required when you create the androidDeviceOwnerPkcsCertificateProfile.</span></span>

|<span data-ttu-id="89289-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="89289-130">Property</span></span>|<span data-ttu-id="89289-131">Тип</span><span class="sxs-lookup"><span data-stu-id="89289-131">Type</span></span>|<span data-ttu-id="89289-132">Описание</span><span class="sxs-lookup"><span data-stu-id="89289-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89289-133">id</span><span class="sxs-lookup"><span data-stu-id="89289-133">id</span></span>|<span data-ttu-id="89289-134">String</span><span class="sxs-lookup"><span data-stu-id="89289-134">String</span></span>|<span data-ttu-id="89289-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89289-135">Key of the entity.</span></span> <span data-ttu-id="89289-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89289-137">lastModifiedDateTime</span></span>|<span data-ttu-id="89289-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89289-138">DateTimeOffset</span></span>|<span data-ttu-id="89289-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89289-139">DateTime the object was last modified.</span></span> <span data-ttu-id="89289-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89289-141">roleScopeTagIds</span></span>|<span data-ttu-id="89289-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89289-142">String collection</span></span>|<span data-ttu-id="89289-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="89289-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89289-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="89289-145">supportsScopeTags</span></span>|<span data-ttu-id="89289-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="89289-146">Boolean</span></span>|<span data-ttu-id="89289-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="89289-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89289-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="89289-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89289-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="89289-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89289-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89289-150">This property is read-only.</span></span> <span data-ttu-id="89289-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89289-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="89289-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89289-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="89289-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="89289-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="89289-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89289-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="89289-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89289-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="89289-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="89289-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="89289-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89289-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="89289-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89289-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="89289-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="89289-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="89289-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89289-164">createdDateTime</span></span>|<span data-ttu-id="89289-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89289-165">DateTimeOffset</span></span>|<span data-ttu-id="89289-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="89289-166">DateTime the object was created.</span></span> <span data-ttu-id="89289-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-168">description</span><span class="sxs-lookup"><span data-stu-id="89289-168">description</span></span>|<span data-ttu-id="89289-169">String</span><span class="sxs-lookup"><span data-stu-id="89289-169">String</span></span>|<span data-ttu-id="89289-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89289-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89289-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-172">displayName</span><span class="sxs-lookup"><span data-stu-id="89289-172">displayName</span></span>|<span data-ttu-id="89289-173">String</span><span class="sxs-lookup"><span data-stu-id="89289-173">String</span></span>|<span data-ttu-id="89289-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89289-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89289-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-176">version</span><span class="sxs-lookup"><span data-stu-id="89289-176">version</span></span>|<span data-ttu-id="89289-177">Int32</span><span class="sxs-lookup"><span data-stu-id="89289-177">Int32</span></span>|<span data-ttu-id="89289-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89289-178">Version of the device configuration.</span></span> <span data-ttu-id="89289-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89289-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89289-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="89289-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="89289-181">Int32</span><span class="sxs-lookup"><span data-stu-id="89289-181">Int32</span></span>|<span data-ttu-id="89289-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="89289-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="89289-183">Допустимые значения — от 1 до 99, наследуемые от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89289-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89289-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89289-184">subjectNameFormat</span></span>|[<span data-ttu-id="89289-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89289-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="89289-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="89289-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="89289-187">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="89289-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="89289-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="89289-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="89289-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="89289-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="89289-190">Int32</span><span class="sxs-lookup"><span data-stu-id="89289-190">Int32</span></span>|<span data-ttu-id="89289-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="89289-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="89289-192">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89289-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89289-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89289-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="89289-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89289-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="89289-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="89289-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="89289-196">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="89289-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="89289-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="89289-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="89289-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="89289-198">extendedKeyUsages</span></span>|<span data-ttu-id="89289-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="89289-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="89289-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="89289-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="89289-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="89289-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="89289-202">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89289-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89289-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89289-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="89289-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89289-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="89289-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="89289-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="89289-206">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="89289-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="89289-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="89289-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="89289-208">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="89289-208">certificationAuthority</span></span>|<span data-ttu-id="89289-209">String</span><span class="sxs-lookup"><span data-stu-id="89289-209">String</span></span>|<span data-ttu-id="89289-210">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="89289-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="89289-211">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="89289-211">certificationAuthorityName</span></span>|<span data-ttu-id="89289-212">String</span><span class="sxs-lookup"><span data-stu-id="89289-212">String</span></span>|<span data-ttu-id="89289-213">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="89289-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="89289-214">цертификатионаусорититипе</span><span class="sxs-lookup"><span data-stu-id="89289-214">certificationAuthorityType</span></span>|[<span data-ttu-id="89289-215">deviceManagementCertificationAuthority</span><span class="sxs-lookup"><span data-stu-id="89289-215">deviceManagementCertificationAuthority</span></span>](../resources/intune-deviceconfig-devicemanagementcertificationauthority.md)|<span data-ttu-id="89289-216">Тип центра сертификации.</span><span class="sxs-lookup"><span data-stu-id="89289-216">Certification authority type.</span></span> <span data-ttu-id="89289-217">Возможные значения: `notConfigured`, `microsoft`, `digiCert`.</span><span class="sxs-lookup"><span data-stu-id="89289-217">Possible values are: `notConfigured`, `microsoft`, `digiCert`.</span></span>|
|<span data-ttu-id="89289-218">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="89289-218">certificateTemplateName</span></span>|<span data-ttu-id="89289-219">String</span><span class="sxs-lookup"><span data-stu-id="89289-219">String</span></span>|<span data-ttu-id="89289-220">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="89289-220">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="89289-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="89289-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="89289-222">String</span><span class="sxs-lookup"><span data-stu-id="89289-222">String</span></span>|<span data-ttu-id="89289-223">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="89289-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="89289-224">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="89289-224">subjectNameFormatString</span></span>|<span data-ttu-id="89289-225">String</span><span class="sxs-lookup"><span data-stu-id="89289-225">String</span></span>|<span data-ttu-id="89289-226">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="89289-226">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="89289-227">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="89289-227">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="89289-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89289-228">certificateStore</span></span>|[<span data-ttu-id="89289-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="89289-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="89289-230">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="89289-230">Target store certificate.</span></span> <span data-ttu-id="89289-231">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="89289-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="89289-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="89289-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="89289-233">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="89289-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="89289-234">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="89289-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="89289-235">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="89289-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="89289-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="89289-236">Response</span></span>
<span data-ttu-id="89289-237">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерпкксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89289-237">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89289-238">Пример</span><span class="sxs-lookup"><span data-stu-id="89289-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="89289-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="89289-239">Request</span></span>
<span data-ttu-id="89289-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89289-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2078

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerPkcsCertificateProfile",
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
  "certificationAuthorityType": "microsoft",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
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

### <a name="response"></a><span data-ttu-id="89289-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="89289-241">Response</span></span>
<span data-ttu-id="89289-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89289-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2250

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerPkcsCertificateProfile",
  "id": "5e86a0e6-a0e6-5e86-e6a0-865ee6a0865e",
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
  "certificationAuthorityType": "microsoft",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
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






