---
title: Создание androidScepCertificateProfile
description: Создание нового объекта androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 696cb17ae1d6fc829c3a9426e7493ddc9f12e10f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969934"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="94c14-103">Создание androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="94c14-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="94c14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94c14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94c14-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94c14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94c14-106">Создание нового объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="94c14-106">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94c14-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94c14-107">Prerequisites</span></span>
<span data-ttu-id="94c14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94c14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94c14-110">Permission type</span></span>|<span data-ttu-id="94c14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94c14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94c14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94c14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94c14-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c14-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94c14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94c14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94c14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94c14-115">Not supported.</span></span>|
|<span data-ttu-id="94c14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94c14-116">Application</span></span>|<span data-ttu-id="94c14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94c14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94c14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94c14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="94c14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94c14-119">Request headers</span></span>
|<span data-ttu-id="94c14-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94c14-120">Header</span></span>|<span data-ttu-id="94c14-121">Значение</span><span class="sxs-lookup"><span data-stu-id="94c14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94c14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94c14-122">Authorization</span></span>|<span data-ttu-id="94c14-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94c14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94c14-124">Accept</span><span class="sxs-lookup"><span data-stu-id="94c14-124">Accept</span></span>|<span data-ttu-id="94c14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94c14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94c14-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94c14-126">Request body</span></span>
<span data-ttu-id="94c14-127">В тексте запроса добавьте представление объекта androidScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94c14-127">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="94c14-128">В следующей таблице приведены свойства, необходимые при создании androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="94c14-128">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="94c14-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="94c14-129">Property</span></span>|<span data-ttu-id="94c14-130">Тип</span><span class="sxs-lookup"><span data-stu-id="94c14-130">Type</span></span>|<span data-ttu-id="94c14-131">Описание</span><span class="sxs-lookup"><span data-stu-id="94c14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c14-132">id</span><span class="sxs-lookup"><span data-stu-id="94c14-132">id</span></span>|<span data-ttu-id="94c14-133">String</span><span class="sxs-lookup"><span data-stu-id="94c14-133">String</span></span>|<span data-ttu-id="94c14-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="94c14-134">Key of the entity.</span></span> <span data-ttu-id="94c14-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94c14-136">lastModifiedDateTime</span></span>|<span data-ttu-id="94c14-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c14-137">DateTimeOffset</span></span>|<span data-ttu-id="94c14-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="94c14-138">DateTime the object was last modified.</span></span> <span data-ttu-id="94c14-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94c14-140">roleScopeTagIds</span></span>|<span data-ttu-id="94c14-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="94c14-141">String collection</span></span>|<span data-ttu-id="94c14-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="94c14-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="94c14-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="94c14-144">supportsScopeTags</span></span>|<span data-ttu-id="94c14-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="94c14-145">Boolean</span></span>|<span data-ttu-id="94c14-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="94c14-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="94c14-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="94c14-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="94c14-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="94c14-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="94c14-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94c14-149">This property is read-only.</span></span> <span data-ttu-id="94c14-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="94c14-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="94c14-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="94c14-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="94c14-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="94c14-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="94c14-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="94c14-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="94c14-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="94c14-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="94c14-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="94c14-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="94c14-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="94c14-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="94c14-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="94c14-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="94c14-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="94c14-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="94c14-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94c14-163">createdDateTime</span></span>|<span data-ttu-id="94c14-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c14-164">DateTimeOffset</span></span>|<span data-ttu-id="94c14-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="94c14-165">DateTime the object was created.</span></span> <span data-ttu-id="94c14-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-167">description</span><span class="sxs-lookup"><span data-stu-id="94c14-167">description</span></span>|<span data-ttu-id="94c14-168">String</span><span class="sxs-lookup"><span data-stu-id="94c14-168">String</span></span>|<span data-ttu-id="94c14-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="94c14-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="94c14-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-171">displayName</span><span class="sxs-lookup"><span data-stu-id="94c14-171">displayName</span></span>|<span data-ttu-id="94c14-172">Строка</span><span class="sxs-lookup"><span data-stu-id="94c14-172">String</span></span>|<span data-ttu-id="94c14-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="94c14-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="94c14-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-175">version</span><span class="sxs-lookup"><span data-stu-id="94c14-175">version</span></span>|<span data-ttu-id="94c14-176">Int32</span><span class="sxs-lookup"><span data-stu-id="94c14-176">Int32</span></span>|<span data-ttu-id="94c14-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="94c14-177">Version of the device configuration.</span></span> <span data-ttu-id="94c14-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94c14-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="94c14-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="94c14-180">Int32</span><span class="sxs-lookup"><span data-stu-id="94c14-180">Int32</span></span>|<span data-ttu-id="94c14-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="94c14-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="94c14-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="94c14-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="94c14-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="94c14-183">subjectNameFormat</span></span>|[<span data-ttu-id="94c14-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="94c14-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="94c14-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="94c14-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="94c14-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="94c14-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="94c14-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="94c14-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="94c14-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="94c14-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="94c14-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="94c14-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="94c14-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="94c14-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="94c14-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="94c14-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="94c14-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="94c14-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="94c14-194">Int32</span><span class="sxs-lookup"><span data-stu-id="94c14-194">Int32</span></span>|<span data-ttu-id="94c14-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="94c14-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="94c14-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="94c14-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="94c14-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="94c14-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="94c14-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="94c14-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="94c14-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="94c14-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="94c14-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94c14-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="94c14-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="94c14-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="94c14-202">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="94c14-202">extendedKeyUsages</span></span>|<span data-ttu-id="94c14-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="94c14-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="94c14-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="94c14-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="94c14-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="94c14-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="94c14-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="94c14-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="94c14-207">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="94c14-207">scepServerUrls</span></span>|<span data-ttu-id="94c14-208">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="94c14-208">String collection</span></span>|<span data-ttu-id="94c14-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="94c14-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="94c14-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="94c14-210">subjectNameFormatString</span></span>|<span data-ttu-id="94c14-211">String</span><span class="sxs-lookup"><span data-stu-id="94c14-211">String</span></span>|<span data-ttu-id="94c14-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="94c14-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="94c14-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="94c14-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="94c14-214">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="94c14-214">keyUsage</span></span>|[<span data-ttu-id="94c14-215">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="94c14-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="94c14-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="94c14-216">SCEP Key Usage.</span></span> <span data-ttu-id="94c14-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="94c14-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="94c14-218">keySize</span><span class="sxs-lookup"><span data-stu-id="94c14-218">keySize</span></span>|[<span data-ttu-id="94c14-219">keySize</span><span class="sxs-lookup"><span data-stu-id="94c14-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="94c14-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="94c14-220">SCEP Key Size.</span></span> <span data-ttu-id="94c14-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="94c14-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="94c14-222">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="94c14-222">hashAlgorithm</span></span>|[<span data-ttu-id="94c14-223">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="94c14-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="94c14-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="94c14-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="94c14-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="94c14-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="94c14-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="94c14-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="94c14-227">String</span><span class="sxs-lookup"><span data-stu-id="94c14-227">String</span></span>|<span data-ttu-id="94c14-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="94c14-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="94c14-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="94c14-229">Response</span></span>
<span data-ttu-id="94c14-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94c14-230">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94c14-231">Пример</span><span class="sxs-lookup"><span data-stu-id="94c14-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="94c14-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="94c14-232">Request</span></span>
<span data-ttu-id="94c14-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94c14-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="94c14-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="94c14-234">Response</span></span>
<span data-ttu-id="94c14-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94c14-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





