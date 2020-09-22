---
title: Создание Андроидворкпрофилесцепцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилесцепцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 675a6a2404f3275fbbe1a72c1479d60a2660b4fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990272"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="f6e3c-103">Создание Андроидворкпрофилесцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="f6e3c-103">Create androidWorkProfileScepCertificateProfile</span></span>

<span data-ttu-id="f6e3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6e3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6e3c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6e3c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6e3c-107">Создание нового объекта [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f6e3c-107">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6e3c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6e3c-108">Prerequisites</span></span>
<span data-ttu-id="f6e3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6e3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6e3c-111">Permission type</span></span>|<span data-ttu-id="f6e3c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6e3c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6e3c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e3c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6e3c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6e3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-116">Not supported.</span></span>|
|<span data-ttu-id="f6e3c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6e3c-117">Application</span></span>|<span data-ttu-id="f6e3c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e3c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6e3c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6e3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6e3c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6e3c-120">Request headers</span></span>
|<span data-ttu-id="f6e3c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6e3c-121">Header</span></span>|<span data-ttu-id="f6e3c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6e3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6e3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6e3c-123">Authorization</span></span>|<span data-ttu-id="f6e3c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6e3c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6e3c-125">Accept</span></span>|<span data-ttu-id="f6e3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6e3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6e3c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6e3c-127">Request body</span></span>
<span data-ttu-id="f6e3c-128">В тексте запроса добавьте представление объекта Андроидворкпрофилесцепцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-128">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="f6e3c-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилесцепцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-129">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="f6e3c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6e3c-130">Property</span></span>|<span data-ttu-id="f6e3c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6e3c-131">Type</span></span>|<span data-ttu-id="f6e3c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6e3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e3c-133">id</span><span class="sxs-lookup"><span data-stu-id="f6e3c-133">id</span></span>|<span data-ttu-id="f6e3c-134">String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-134">String</span></span>|<span data-ttu-id="f6e3c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-135">Key of the entity.</span></span> <span data-ttu-id="f6e3c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6e3c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f6e3c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6e3c-138">DateTimeOffset</span></span>|<span data-ttu-id="f6e3c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f6e3c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6e3c-141">roleScopeTagIds</span></span>|<span data-ttu-id="f6e3c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-142">String collection</span></span>|<span data-ttu-id="f6e3c-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6e3c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f6e3c-145">supportsScopeTags</span></span>|<span data-ttu-id="f6e3c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6e3c-146">Boolean</span></span>|<span data-ttu-id="f6e3c-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f6e3c-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f6e3c-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f6e3c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-150">This property is read-only.</span></span> <span data-ttu-id="f6e3c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6e3c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f6e3c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6e3c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f6e3c-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f6e3c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6e3c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f6e3c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6e3c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f6e3c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f6e3c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6e3c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f6e3c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6e3c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f6e3c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f6e3c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6e3c-164">createdDateTime</span></span>|<span data-ttu-id="f6e3c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6e3c-165">DateTimeOffset</span></span>|<span data-ttu-id="f6e3c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-166">DateTime the object was created.</span></span> <span data-ttu-id="f6e3c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-168">description</span><span class="sxs-lookup"><span data-stu-id="f6e3c-168">description</span></span>|<span data-ttu-id="f6e3c-169">String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-169">String</span></span>|<span data-ttu-id="f6e3c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6e3c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f6e3c-172">displayName</span></span>|<span data-ttu-id="f6e3c-173">String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-173">String</span></span>|<span data-ttu-id="f6e3c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6e3c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-176">version</span><span class="sxs-lookup"><span data-stu-id="f6e3c-176">version</span></span>|<span data-ttu-id="f6e3c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e3c-177">Int32</span></span>|<span data-ttu-id="f6e3c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-178">Version of the device configuration.</span></span> <span data-ttu-id="f6e3c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6e3c-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="f6e3c-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f6e3c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e3c-181">Int32</span></span>|<span data-ttu-id="f6e3c-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f6e3c-183">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f6e3c-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f6e3c-184">subjectNameFormat</span></span>|[<span data-ttu-id="f6e3c-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f6e3c-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f6e3c-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f6e3c-187">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f6e3c-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f6e3c-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f6e3c-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f6e3c-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e3c-190">Int32</span></span>|<span data-ttu-id="f6e3c-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f6e3c-192">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f6e3c-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f6e3c-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f6e3c-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f6e3c-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f6e3c-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f6e3c-196">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f6e3c-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f6e3c-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="f6e3c-198">extendedKeyUsages</span></span>|<span data-ttu-id="f6e3c-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f6e3c-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f6e3c-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f6e3c-202">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f6e3c-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f6e3c-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f6e3c-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f6e3c-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f6e3c-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f6e3c-206">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f6e3c-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f6e3c-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f6e3c-208">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="f6e3c-208">scepServerUrls</span></span>|<span data-ttu-id="f6e3c-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-209">String collection</span></span>|<span data-ttu-id="f6e3c-210">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="f6e3c-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="f6e3c-211">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="f6e3c-211">subjectNameFormatString</span></span>|<span data-ttu-id="f6e3c-212">String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-212">String</span></span>|<span data-ttu-id="f6e3c-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f6e3c-214">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="f6e3c-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f6e3c-215">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="f6e3c-215">keyUsage</span></span>|[<span data-ttu-id="f6e3c-216">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="f6e3c-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f6e3c-217">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-217">SCEP Key Usage.</span></span> <span data-ttu-id="f6e3c-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f6e3c-219">keySize</span><span class="sxs-lookup"><span data-stu-id="f6e3c-219">keySize</span></span>|[<span data-ttu-id="f6e3c-220">keySize</span><span class="sxs-lookup"><span data-stu-id="f6e3c-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f6e3c-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-221">SCEP Key Size.</span></span> <span data-ttu-id="f6e3c-222">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="f6e3c-223">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="f6e3c-223">hashAlgorithm</span></span>|[<span data-ttu-id="f6e3c-224">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="f6e3c-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f6e3c-225">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f6e3c-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f6e3c-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f6e3c-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f6e3c-228">String</span><span class="sxs-lookup"><span data-stu-id="f6e3c-228">String</span></span>|<span data-ttu-id="f6e3c-229">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f6e3c-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f6e3c-230">certificateStore</span></span>|[<span data-ttu-id="f6e3c-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f6e3c-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f6e3c-232">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-232">Target store certificate.</span></span> <span data-ttu-id="f6e3c-233">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f6e3c-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f6e3c-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f6e3c-235">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f6e3c-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f6e3c-236">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f6e3c-237">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f6e3c-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6e3c-238">Response</span></span>
<span data-ttu-id="f6e3c-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-239">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6e3c-240">Пример</span><span class="sxs-lookup"><span data-stu-id="f6e3c-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6e3c-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6e3c-241">Request</span></span>
<span data-ttu-id="f6e3c-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="f6e3c-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6e3c-243">Response</span></span>
<span data-ttu-id="f6e3c-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6e3c-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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






