---
title: Создание androidScepCertificateProfile
description: Создание нового объекта androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34d22aea71cfb1990c4efade33450e4da3fe6d79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311496"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="1cabf-103">Создание androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="1cabf-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="1cabf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cabf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cabf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cabf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cabf-106">Создание нового объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1cabf-106">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cabf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cabf-107">Prerequisites</span></span>
<span data-ttu-id="1cabf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cabf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cabf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cabf-110">Permission type</span></span>|<span data-ttu-id="1cabf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cabf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cabf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cabf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cabf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cabf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cabf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cabf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cabf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cabf-115">Not supported.</span></span>|
|<span data-ttu-id="1cabf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cabf-116">Application</span></span>|<span data-ttu-id="1cabf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cabf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cabf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cabf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1cabf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cabf-119">Request headers</span></span>
|<span data-ttu-id="1cabf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cabf-120">Header</span></span>|<span data-ttu-id="1cabf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1cabf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cabf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cabf-122">Authorization</span></span>|<span data-ttu-id="1cabf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cabf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cabf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1cabf-124">Accept</span></span>|<span data-ttu-id="1cabf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cabf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cabf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cabf-126">Request body</span></span>
<span data-ttu-id="1cabf-127">В тексте запроса добавьте представление объекта androidScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cabf-127">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="1cabf-128">В следующей таблице приведены свойства, необходимые при создании androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1cabf-128">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="1cabf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cabf-129">Property</span></span>|<span data-ttu-id="1cabf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1cabf-130">Type</span></span>|<span data-ttu-id="1cabf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1cabf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cabf-132">id</span><span class="sxs-lookup"><span data-stu-id="1cabf-132">id</span></span>|<span data-ttu-id="1cabf-133">String</span><span class="sxs-lookup"><span data-stu-id="1cabf-133">String</span></span>|<span data-ttu-id="1cabf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cabf-134">Key of the entity.</span></span> <span data-ttu-id="1cabf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cabf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1cabf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cabf-137">DateTimeOffset</span></span>|<span data-ttu-id="1cabf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1cabf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1cabf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cabf-140">roleScopeTagIds</span></span>|<span data-ttu-id="1cabf-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1cabf-141">String collection</span></span>|<span data-ttu-id="1cabf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1cabf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1cabf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1cabf-144">supportsScopeTags</span></span>|<span data-ttu-id="1cabf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cabf-145">Boolean</span></span>|<span data-ttu-id="1cabf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1cabf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1cabf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1cabf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1cabf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1cabf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1cabf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cabf-149">This property is read-only.</span></span> <span data-ttu-id="1cabf-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1cabf-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1cabf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1cabf-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1cabf-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1cabf-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1cabf-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1cabf-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1cabf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1cabf-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1cabf-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1cabf-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1cabf-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1cabf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1cabf-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1cabf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1cabf-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1cabf-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1cabf-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cabf-163">createdDateTime</span></span>|<span data-ttu-id="1cabf-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cabf-164">DateTimeOffset</span></span>|<span data-ttu-id="1cabf-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1cabf-165">DateTime the object was created.</span></span> <span data-ttu-id="1cabf-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-167">description</span><span class="sxs-lookup"><span data-stu-id="1cabf-167">description</span></span>|<span data-ttu-id="1cabf-168">String</span><span class="sxs-lookup"><span data-stu-id="1cabf-168">String</span></span>|<span data-ttu-id="1cabf-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cabf-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1cabf-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1cabf-171">displayName</span></span>|<span data-ttu-id="1cabf-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1cabf-172">String</span></span>|<span data-ttu-id="1cabf-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cabf-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1cabf-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-175">version</span><span class="sxs-lookup"><span data-stu-id="1cabf-175">version</span></span>|<span data-ttu-id="1cabf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1cabf-176">Int32</span></span>|<span data-ttu-id="1cabf-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cabf-177">Version of the device configuration.</span></span> <span data-ttu-id="1cabf-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cabf-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="1cabf-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="1cabf-180">Int32</span><span class="sxs-lookup"><span data-stu-id="1cabf-180">Int32</span></span>|<span data-ttu-id="1cabf-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cabf-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1cabf-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cabf-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cabf-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1cabf-183">subjectNameFormat</span></span>|[<span data-ttu-id="1cabf-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1cabf-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1cabf-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cabf-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="1cabf-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cabf-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1cabf-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1cabf-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1cabf-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1cabf-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1cabf-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cabf-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1cabf-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cabf-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1cabf-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1cabf-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1cabf-194">Int32</span><span class="sxs-lookup"><span data-stu-id="1cabf-194">Int32</span></span>|<span data-ttu-id="1cabf-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cabf-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="1cabf-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cabf-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cabf-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cabf-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1cabf-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cabf-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1cabf-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1cabf-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1cabf-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cabf-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1cabf-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1cabf-202">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="1cabf-202">extendedKeyUsages</span></span>|<span data-ttu-id="1cabf-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="1cabf-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="1cabf-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="1cabf-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="1cabf-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1cabf-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1cabf-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1cabf-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1cabf-207">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="1cabf-207">scepServerUrls</span></span>|<span data-ttu-id="1cabf-208">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1cabf-208">String collection</span></span>|<span data-ttu-id="1cabf-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="1cabf-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="1cabf-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="1cabf-210">subjectNameFormatString</span></span>|<span data-ttu-id="1cabf-211">String</span><span class="sxs-lookup"><span data-stu-id="1cabf-211">String</span></span>|<span data-ttu-id="1cabf-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="1cabf-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="1cabf-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="1cabf-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="1cabf-214">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="1cabf-214">keyUsage</span></span>|[<span data-ttu-id="1cabf-215">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="1cabf-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="1cabf-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="1cabf-216">SCEP Key Usage.</span></span> <span data-ttu-id="1cabf-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="1cabf-218">keySize</span><span class="sxs-lookup"><span data-stu-id="1cabf-218">keySize</span></span>|[<span data-ttu-id="1cabf-219">keySize</span><span class="sxs-lookup"><span data-stu-id="1cabf-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="1cabf-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="1cabf-220">SCEP Key Size.</span></span> <span data-ttu-id="1cabf-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="1cabf-222">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="1cabf-222">hashAlgorithm</span></span>|[<span data-ttu-id="1cabf-223">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="1cabf-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="1cabf-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="1cabf-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="1cabf-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="1cabf-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="1cabf-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="1cabf-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="1cabf-227">String</span><span class="sxs-lookup"><span data-stu-id="1cabf-227">String</span></span>|<span data-ttu-id="1cabf-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="1cabf-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="1cabf-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cabf-229">Response</span></span>
<span data-ttu-id="1cabf-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cabf-230">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cabf-231">Пример</span><span class="sxs-lookup"><span data-stu-id="1cabf-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cabf-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cabf-232">Request</span></span>
<span data-ttu-id="1cabf-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cabf-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1cabf-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cabf-234">Response</span></span>
<span data-ttu-id="1cabf-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cabf-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






