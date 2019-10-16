---
title: Создание Андроидворкпрофилепкксцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилепкксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53935778ef12d5bbb5c59751af83fc7c7a2c4dc6
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534290"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="3737f-103">Создание Андроидворкпрофилепкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="3737f-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="3737f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3737f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3737f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3737f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3737f-106">Создание нового объекта [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3737f-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3737f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3737f-107">Prerequisites</span></span>
<span data-ttu-id="3737f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3737f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3737f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3737f-110">Permission type</span></span>|<span data-ttu-id="3737f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3737f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3737f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3737f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3737f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3737f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3737f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3737f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3737f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3737f-115">Not supported.</span></span>|
|<span data-ttu-id="3737f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3737f-116">Application</span></span>|<span data-ttu-id="3737f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3737f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3737f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3737f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3737f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3737f-119">Request headers</span></span>
|<span data-ttu-id="3737f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3737f-120">Header</span></span>|<span data-ttu-id="3737f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3737f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3737f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3737f-122">Authorization</span></span>|<span data-ttu-id="3737f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3737f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3737f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3737f-124">Accept</span></span>|<span data-ttu-id="3737f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3737f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3737f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3737f-126">Request body</span></span>
<span data-ttu-id="3737f-127">В тексте запроса добавьте представление объекта Андроидворкпрофилепкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3737f-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="3737f-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилепкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="3737f-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="3737f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3737f-129">Property</span></span>|<span data-ttu-id="3737f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3737f-130">Type</span></span>|<span data-ttu-id="3737f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3737f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3737f-132">id</span><span class="sxs-lookup"><span data-stu-id="3737f-132">id</span></span>|<span data-ttu-id="3737f-133">String</span><span class="sxs-lookup"><span data-stu-id="3737f-133">String</span></span>|<span data-ttu-id="3737f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3737f-134">Key of the entity.</span></span> <span data-ttu-id="3737f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3737f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3737f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3737f-137">DateTimeOffset</span></span>|<span data-ttu-id="3737f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3737f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3737f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3737f-140">roleScopeTagIds</span></span>|<span data-ttu-id="3737f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3737f-141">String collection</span></span>|<span data-ttu-id="3737f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3737f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3737f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3737f-144">supportsScopeTags</span></span>|<span data-ttu-id="3737f-145">Логический</span><span class="sxs-lookup"><span data-stu-id="3737f-145">Boolean</span></span>|<span data-ttu-id="3737f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3737f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3737f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3737f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3737f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3737f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3737f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3737f-149">This property is read-only.</span></span> <span data-ttu-id="3737f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3737f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3737f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3737f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3737f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3737f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3737f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3737f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3737f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3737f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3737f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3737f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3737f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3737f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3737f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3737f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3737f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3737f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3737f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3737f-163">createdDateTime</span></span>|<span data-ttu-id="3737f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3737f-164">DateTimeOffset</span></span>|<span data-ttu-id="3737f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3737f-165">DateTime the object was created.</span></span> <span data-ttu-id="3737f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-167">description</span><span class="sxs-lookup"><span data-stu-id="3737f-167">description</span></span>|<span data-ttu-id="3737f-168">String</span><span class="sxs-lookup"><span data-stu-id="3737f-168">String</span></span>|<span data-ttu-id="3737f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3737f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3737f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3737f-171">displayName</span></span>|<span data-ttu-id="3737f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="3737f-172">String</span></span>|<span data-ttu-id="3737f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3737f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3737f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-175">version</span><span class="sxs-lookup"><span data-stu-id="3737f-175">version</span></span>|<span data-ttu-id="3737f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3737f-176">Int32</span></span>|<span data-ttu-id="3737f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3737f-177">Version of the device configuration.</span></span> <span data-ttu-id="3737f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3737f-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="3737f-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="3737f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="3737f-180">Int32</span></span>|<span data-ttu-id="3737f-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="3737f-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3737f-182">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3737f-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3737f-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3737f-183">subjectNameFormat</span></span>|[<span data-ttu-id="3737f-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3737f-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3737f-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3737f-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="3737f-186">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3737f-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3737f-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3737f-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3737f-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3737f-189">Int32</span><span class="sxs-lookup"><span data-stu-id="3737f-189">Int32</span></span>|<span data-ttu-id="3737f-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3737f-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3737f-191">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3737f-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3737f-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3737f-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3737f-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3737f-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3737f-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3737f-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3737f-195">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3737f-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3737f-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3737f-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="3737f-197">extendedKeyUsages</span></span>|<span data-ttu-id="3737f-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="3737f-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3737f-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="3737f-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3737f-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3737f-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3737f-201">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3737f-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3737f-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3737f-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3737f-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3737f-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3737f-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3737f-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3737f-205">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3737f-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3737f-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3737f-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3737f-207">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="3737f-207">certificationAuthority</span></span>|<span data-ttu-id="3737f-208">String</span><span class="sxs-lookup"><span data-stu-id="3737f-208">String</span></span>|<span data-ttu-id="3737f-209">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3737f-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="3737f-210">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="3737f-210">certificationAuthorityName</span></span>|<span data-ttu-id="3737f-211">String</span><span class="sxs-lookup"><span data-stu-id="3737f-211">String</span></span>|<span data-ttu-id="3737f-212">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3737f-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="3737f-213">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="3737f-213">certificateTemplateName</span></span>|<span data-ttu-id="3737f-214">String</span><span class="sxs-lookup"><span data-stu-id="3737f-214">String</span></span>|<span data-ttu-id="3737f-215">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="3737f-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="3737f-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3737f-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3737f-217">String</span><span class="sxs-lookup"><span data-stu-id="3737f-217">String</span></span>|<span data-ttu-id="3737f-218">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="3737f-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3737f-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="3737f-219">Response</span></span>
<span data-ttu-id="3737f-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3737f-220">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3737f-221">Пример</span><span class="sxs-lookup"><span data-stu-id="3737f-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="3737f-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="3737f-222">Request</span></span>
<span data-ttu-id="3737f-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3737f-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3737f-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="3737f-224">Response</span></span>
<span data-ttu-id="3737f-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3737f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






