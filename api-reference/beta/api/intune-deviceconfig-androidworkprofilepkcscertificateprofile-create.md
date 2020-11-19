---
title: Создание Андроидворкпрофилепкксцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилепкксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f82c16538499aafa5e5b104dd140f95d9b9b1d28
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49237361"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="02237-103">Создание Андроидворкпрофилепкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="02237-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

<span data-ttu-id="02237-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02237-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02237-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02237-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02237-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02237-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02237-107">Создание нового объекта [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="02237-107">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02237-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02237-108">Prerequisites</span></span>
<span data-ttu-id="02237-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02237-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02237-111">Permission type</span></span>|<span data-ttu-id="02237-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02237-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02237-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02237-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02237-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02237-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02237-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02237-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02237-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02237-116">Not supported.</span></span>|
|<span data-ttu-id="02237-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="02237-117">Application</span></span>|<span data-ttu-id="02237-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02237-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02237-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02237-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02237-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02237-120">Request headers</span></span>
|<span data-ttu-id="02237-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02237-121">Header</span></span>|<span data-ttu-id="02237-122">Значение</span><span class="sxs-lookup"><span data-stu-id="02237-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02237-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02237-123">Authorization</span></span>|<span data-ttu-id="02237-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02237-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02237-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02237-125">Accept</span></span>|<span data-ttu-id="02237-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02237-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02237-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02237-127">Request body</span></span>
<span data-ttu-id="02237-128">В тексте запроса добавьте представление объекта Андроидворкпрофилепкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02237-128">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="02237-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилепкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="02237-129">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="02237-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="02237-130">Property</span></span>|<span data-ttu-id="02237-131">Тип</span><span class="sxs-lookup"><span data-stu-id="02237-131">Type</span></span>|<span data-ttu-id="02237-132">Описание</span><span class="sxs-lookup"><span data-stu-id="02237-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02237-133">id</span><span class="sxs-lookup"><span data-stu-id="02237-133">id</span></span>|<span data-ttu-id="02237-134">String</span><span class="sxs-lookup"><span data-stu-id="02237-134">String</span></span>|<span data-ttu-id="02237-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="02237-135">Key of the entity.</span></span> <span data-ttu-id="02237-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02237-137">lastModifiedDateTime</span></span>|<span data-ttu-id="02237-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02237-138">DateTimeOffset</span></span>|<span data-ttu-id="02237-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="02237-139">DateTime the object was last modified.</span></span> <span data-ttu-id="02237-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02237-141">roleScopeTagIds</span></span>|<span data-ttu-id="02237-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02237-142">String collection</span></span>|<span data-ttu-id="02237-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="02237-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="02237-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="02237-145">supportsScopeTags</span></span>|<span data-ttu-id="02237-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="02237-146">Boolean</span></span>|<span data-ttu-id="02237-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="02237-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="02237-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="02237-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="02237-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="02237-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="02237-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02237-150">This property is read-only.</span></span> <span data-ttu-id="02237-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="02237-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="02237-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="02237-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="02237-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="02237-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="02237-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="02237-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="02237-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="02237-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="02237-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="02237-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="02237-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="02237-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="02237-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="02237-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="02237-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="02237-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="02237-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02237-164">createdDateTime</span></span>|<span data-ttu-id="02237-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02237-165">DateTimeOffset</span></span>|<span data-ttu-id="02237-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="02237-166">DateTime the object was created.</span></span> <span data-ttu-id="02237-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-168">description</span><span class="sxs-lookup"><span data-stu-id="02237-168">description</span></span>|<span data-ttu-id="02237-169">String</span><span class="sxs-lookup"><span data-stu-id="02237-169">String</span></span>|<span data-ttu-id="02237-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02237-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="02237-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-172">displayName</span><span class="sxs-lookup"><span data-stu-id="02237-172">displayName</span></span>|<span data-ttu-id="02237-173">String</span><span class="sxs-lookup"><span data-stu-id="02237-173">String</span></span>|<span data-ttu-id="02237-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02237-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="02237-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-176">version</span><span class="sxs-lookup"><span data-stu-id="02237-176">version</span></span>|<span data-ttu-id="02237-177">Int32</span><span class="sxs-lookup"><span data-stu-id="02237-177">Int32</span></span>|<span data-ttu-id="02237-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02237-178">Version of the device configuration.</span></span> <span data-ttu-id="02237-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02237-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02237-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="02237-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="02237-181">Int32</span><span class="sxs-lookup"><span data-stu-id="02237-181">Int32</span></span>|<span data-ttu-id="02237-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="02237-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="02237-183">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02237-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="02237-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="02237-184">subjectNameFormat</span></span>|[<span data-ttu-id="02237-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="02237-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="02237-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="02237-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="02237-187">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="02237-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="02237-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="02237-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="02237-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="02237-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="02237-190">Int32</span><span class="sxs-lookup"><span data-stu-id="02237-190">Int32</span></span>|<span data-ttu-id="02237-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="02237-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="02237-192">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02237-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="02237-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="02237-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="02237-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="02237-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="02237-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="02237-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="02237-196">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="02237-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="02237-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="02237-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="02237-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="02237-198">extendedKeyUsages</span></span>|<span data-ttu-id="02237-199">Коллекция [екстендедкэйусаже](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="02237-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="02237-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="02237-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="02237-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="02237-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="02237-202">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02237-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="02237-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="02237-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="02237-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="02237-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="02237-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="02237-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="02237-206">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="02237-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="02237-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="02237-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="02237-208">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="02237-208">certificationAuthority</span></span>|<span data-ttu-id="02237-209">String</span><span class="sxs-lookup"><span data-stu-id="02237-209">String</span></span>|<span data-ttu-id="02237-210">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="02237-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="02237-211">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="02237-211">certificationAuthorityName</span></span>|<span data-ttu-id="02237-212">String</span><span class="sxs-lookup"><span data-stu-id="02237-212">String</span></span>|<span data-ttu-id="02237-213">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="02237-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="02237-214">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="02237-214">certificateTemplateName</span></span>|<span data-ttu-id="02237-215">String</span><span class="sxs-lookup"><span data-stu-id="02237-215">String</span></span>|<span data-ttu-id="02237-216">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="02237-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="02237-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="02237-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="02237-218">String</span><span class="sxs-lookup"><span data-stu-id="02237-218">String</span></span>|<span data-ttu-id="02237-219">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="02237-219">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="02237-220">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="02237-220">subjectNameFormatString</span></span>|<span data-ttu-id="02237-221">String</span><span class="sxs-lookup"><span data-stu-id="02237-221">String</span></span>|<span data-ttu-id="02237-222">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="02237-222">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="02237-223">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="02237-223">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="02237-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="02237-224">certificateStore</span></span>|[<span data-ttu-id="02237-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="02237-225">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="02237-226">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="02237-226">Target store certificate.</span></span> <span data-ttu-id="02237-227">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="02237-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="02237-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="02237-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="02237-229">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="02237-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="02237-230">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="02237-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="02237-231">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="02237-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="02237-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="02237-232">Response</span></span>
<span data-ttu-id="02237-233">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02237-233">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02237-234">Пример</span><span class="sxs-lookup"><span data-stu-id="02237-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="02237-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="02237-235">Request</span></span>
<span data-ttu-id="02237-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02237-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2032

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

### <a name="response"></a><span data-ttu-id="02237-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="02237-237">Response</span></span>
<span data-ttu-id="02237-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02237-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2204

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




