---
title: Создание androidForWorkScepCertificateProfile
description: Создание нового объекта androidForWorkScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4697d0393475b09874a93557e2bfc9a9c2a61ac
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176445"
---
# <a name="create-androidforworkscepcertificateprofile"></a><span data-ttu-id="7c936-103">Создание androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7c936-103">Create androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="7c936-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c936-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c936-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c936-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c936-106">Создание нового объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7c936-106">Create a new [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c936-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c936-107">Prerequisites</span></span>
<span data-ttu-id="7c936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c936-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c936-110">Permission type</span></span>|<span data-ttu-id="7c936-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c936-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c936-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c936-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c936-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c936-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c936-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c936-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c936-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c936-115">Not supported.</span></span>|
|<span data-ttu-id="7c936-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c936-116">Application</span></span>|<span data-ttu-id="7c936-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c936-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c936-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c936-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c936-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c936-119">Request headers</span></span>
|<span data-ttu-id="7c936-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c936-120">Header</span></span>|<span data-ttu-id="7c936-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c936-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c936-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c936-122">Authorization</span></span>|<span data-ttu-id="7c936-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c936-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c936-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c936-124">Accept</span></span>|<span data-ttu-id="7c936-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c936-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c936-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c936-126">Request body</span></span>
<span data-ttu-id="7c936-127">В тексте запроса добавьте представление объекта androidForWorkScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c936-127">In the request body, supply a JSON representation for the androidForWorkScepCertificateProfile object.</span></span>

<span data-ttu-id="7c936-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="7c936-128">The following table shows the properties that are required when you create the androidForWorkScepCertificateProfile.</span></span>

|<span data-ttu-id="7c936-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c936-129">Property</span></span>|<span data-ttu-id="7c936-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c936-130">Type</span></span>|<span data-ttu-id="7c936-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c936-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c936-132">id</span><span class="sxs-lookup"><span data-stu-id="7c936-132">id</span></span>|<span data-ttu-id="7c936-133">String</span><span class="sxs-lookup"><span data-stu-id="7c936-133">String</span></span>|<span data-ttu-id="7c936-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7c936-134">Key of the entity.</span></span> <span data-ttu-id="7c936-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c936-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7c936-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c936-137">DateTimeOffset</span></span>|<span data-ttu-id="7c936-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7c936-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7c936-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7c936-140">roleScopeTagIds</span></span>|<span data-ttu-id="7c936-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c936-141">String collection</span></span>|<span data-ttu-id="7c936-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7c936-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7c936-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7c936-144">supportsScopeTags</span></span>|<span data-ttu-id="7c936-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7c936-145">Boolean</span></span>|<span data-ttu-id="7c936-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7c936-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7c936-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7c936-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7c936-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7c936-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7c936-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c936-149">This property is read-only.</span></span> <span data-ttu-id="7c936-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7c936-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7c936-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7c936-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7c936-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7c936-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7c936-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7c936-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7c936-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7c936-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7c936-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7c936-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7c936-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="7c936-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7c936-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="7c936-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7c936-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7c936-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7c936-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c936-163">createdDateTime</span></span>|<span data-ttu-id="7c936-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c936-164">DateTimeOffset</span></span>|<span data-ttu-id="7c936-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7c936-165">DateTime the object was created.</span></span> <span data-ttu-id="7c936-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-167">description</span><span class="sxs-lookup"><span data-stu-id="7c936-167">description</span></span>|<span data-ttu-id="7c936-168">String</span><span class="sxs-lookup"><span data-stu-id="7c936-168">String</span></span>|<span data-ttu-id="7c936-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7c936-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c936-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7c936-171">displayName</span></span>|<span data-ttu-id="7c936-172">Строка</span><span class="sxs-lookup"><span data-stu-id="7c936-172">String</span></span>|<span data-ttu-id="7c936-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7c936-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c936-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-175">version</span><span class="sxs-lookup"><span data-stu-id="7c936-175">version</span></span>|<span data-ttu-id="7c936-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7c936-176">Int32</span></span>|<span data-ttu-id="7c936-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7c936-177">Version of the device configuration.</span></span> <span data-ttu-id="7c936-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c936-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="7c936-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="7c936-180">Int32</span><span class="sxs-lookup"><span data-stu-id="7c936-180">Int32</span></span>|<span data-ttu-id="7c936-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="7c936-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7c936-182">Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7c936-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7c936-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7c936-183">subjectNameFormat</span></span>|[<span data-ttu-id="7c936-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7c936-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="7c936-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7c936-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="7c936-186">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="7c936-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="7c936-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="7c936-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7c936-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7c936-189">Int32</span><span class="sxs-lookup"><span data-stu-id="7c936-189">Int32</span></span>|<span data-ttu-id="7c936-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7c936-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7c936-191">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7c936-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7c936-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7c936-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7c936-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7c936-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7c936-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7c936-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7c936-195">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="7c936-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7c936-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7c936-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="7c936-197">extendedKeyUsages</span></span>|<span data-ttu-id="7c936-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="7c936-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7c936-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="7c936-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7c936-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7c936-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7c936-201">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7c936-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7c936-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7c936-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7c936-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7c936-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7c936-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7c936-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7c936-205">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7c936-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="7c936-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7c936-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7c936-207">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="7c936-207">scepServerUrls</span></span>|<span data-ttu-id="7c936-208">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c936-208">String collection</span></span>|<span data-ttu-id="7c936-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="7c936-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="7c936-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="7c936-210">subjectNameFormatString</span></span>|<span data-ttu-id="7c936-211">String.</span><span class="sxs-lookup"><span data-stu-id="7c936-211">String</span></span>|<span data-ttu-id="7c936-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="7c936-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7c936-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="7c936-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7c936-214">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="7c936-214">keyUsage</span></span>|[<span data-ttu-id="7c936-215">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="7c936-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7c936-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7c936-216">SCEP Key Usage.</span></span> <span data-ttu-id="7c936-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7c936-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7c936-218">keySize</span><span class="sxs-lookup"><span data-stu-id="7c936-218">keySize</span></span>|[<span data-ttu-id="7c936-219">keySize</span><span class="sxs-lookup"><span data-stu-id="7c936-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7c936-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7c936-220">SCEP Key Size.</span></span> <span data-ttu-id="7c936-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7c936-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7c936-222">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="7c936-222">hashAlgorithm</span></span>|[<span data-ttu-id="7c936-223">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="7c936-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="7c936-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="7c936-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="7c936-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="7c936-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="7c936-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7c936-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7c936-227">String.</span><span class="sxs-lookup"><span data-stu-id="7c936-227">String</span></span>|<span data-ttu-id="7c936-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="7c936-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7c936-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7c936-229">certificateStore</span></span>|[<span data-ttu-id="7c936-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7c936-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7c936-231">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="7c936-231">Target store certificate.</span></span> <span data-ttu-id="7c936-232">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="7c936-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7c936-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7c936-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7c936-234">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="7c936-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7c936-235">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="7c936-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="7c936-236">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7c936-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7c936-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c936-237">Response</span></span>
<span data-ttu-id="7c936-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c936-238">If successful, this method returns a `201 Created` response code and a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c936-239">Пример</span><span class="sxs-lookup"><span data-stu-id="7c936-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c936-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c936-240">Request</span></span>
<span data-ttu-id="7c936-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c936-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="7c936-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c936-242">Response</span></span>
<span data-ttu-id="7c936-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c936-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




