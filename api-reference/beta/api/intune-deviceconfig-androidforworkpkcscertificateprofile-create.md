---
title: Создание androidForWorkPkcsCertificateProfile
description: Создание нового объекта androidForWorkPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5170f6c27ea9f4e0eddd1ac016e3f72e3f91cab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435872"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="c01d9-103">Создание androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c01d9-103">Create androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="c01d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c01d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c01d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c01d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c01d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c01d9-107">Создание нового объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c01d9-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c01d9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c01d9-108">Prerequisites</span></span>
<span data-ttu-id="c01d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c01d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c01d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c01d9-111">Permission type</span></span>|<span data-ttu-id="c01d9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c01d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c01d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c01d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c01d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c01d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c01d9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c01d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c01d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01d9-116">Not supported.</span></span>|
|<span data-ttu-id="c01d9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c01d9-117">Application</span></span>|<span data-ttu-id="c01d9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c01d9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c01d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c01d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c01d9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c01d9-120">Request headers</span></span>
|<span data-ttu-id="c01d9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c01d9-121">Header</span></span>|<span data-ttu-id="c01d9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c01d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c01d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c01d9-123">Authorization</span></span>|<span data-ttu-id="c01d9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c01d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c01d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c01d9-125">Accept</span></span>|<span data-ttu-id="c01d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c01d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c01d9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c01d9-127">Request body</span></span>
<span data-ttu-id="c01d9-128">В тексте запроса добавьте представление объекта androidForWorkPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c01d9-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="c01d9-129">В следующей таблице приведены свойства, необходимые при создании androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c01d9-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="c01d9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c01d9-130">Property</span></span>|<span data-ttu-id="c01d9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c01d9-131">Type</span></span>|<span data-ttu-id="c01d9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c01d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01d9-133">id</span><span class="sxs-lookup"><span data-stu-id="c01d9-133">id</span></span>|<span data-ttu-id="c01d9-134">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-134">String</span></span>|<span data-ttu-id="c01d9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c01d9-135">Key of the entity.</span></span> <span data-ttu-id="c01d9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c01d9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c01d9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c01d9-138">DateTimeOffset</span></span>|<span data-ttu-id="c01d9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c01d9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c01d9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c01d9-141">roleScopeTagIds</span></span>|<span data-ttu-id="c01d9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c01d9-142">String collection</span></span>|<span data-ttu-id="c01d9-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c01d9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c01d9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c01d9-145">supportsScopeTags</span></span>|<span data-ttu-id="c01d9-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="c01d9-146">Boolean</span></span>|<span data-ttu-id="c01d9-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c01d9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c01d9-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c01d9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c01d9-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c01d9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c01d9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c01d9-150">This property is read-only.</span></span> <span data-ttu-id="c01d9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c01d9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c01d9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c01d9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c01d9-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c01d9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c01d9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c01d9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c01d9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c01d9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c01d9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c01d9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c01d9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c01d9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c01d9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c01d9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c01d9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c01d9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c01d9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c01d9-164">createdDateTime</span></span>|<span data-ttu-id="c01d9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c01d9-165">DateTimeOffset</span></span>|<span data-ttu-id="c01d9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c01d9-166">DateTime the object was created.</span></span> <span data-ttu-id="c01d9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-168">description</span><span class="sxs-lookup"><span data-stu-id="c01d9-168">description</span></span>|<span data-ttu-id="c01d9-169">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-169">String</span></span>|<span data-ttu-id="c01d9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c01d9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c01d9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c01d9-172">displayName</span></span>|<span data-ttu-id="c01d9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c01d9-173">String</span></span>|<span data-ttu-id="c01d9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c01d9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c01d9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-176">version</span><span class="sxs-lookup"><span data-stu-id="c01d9-176">version</span></span>|<span data-ttu-id="c01d9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c01d9-177">Int32</span></span>|<span data-ttu-id="c01d9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c01d9-178">Version of the device configuration.</span></span> <span data-ttu-id="c01d9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c01d9-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c01d9-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c01d9-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c01d9-181">Int32</span></span>|<span data-ttu-id="c01d9-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c01d9-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c01d9-183">Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c01d9-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c01d9-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c01d9-184">subjectNameFormat</span></span>|[<span data-ttu-id="c01d9-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c01d9-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c01d9-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c01d9-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="c01d9-187">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c01d9-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c01d9-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c01d9-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c01d9-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c01d9-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c01d9-190">Int32</span></span>|<span data-ttu-id="c01d9-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c01d9-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c01d9-192">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c01d9-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c01d9-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c01d9-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c01d9-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c01d9-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c01d9-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c01d9-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c01d9-196">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c01d9-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c01d9-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c01d9-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c01d9-198">extendedKeyUsages</span></span>|<span data-ttu-id="c01d9-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c01d9-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c01d9-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c01d9-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c01d9-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c01d9-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c01d9-202">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c01d9-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c01d9-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c01d9-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c01d9-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c01d9-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c01d9-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c01d9-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c01d9-206">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c01d9-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c01d9-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c01d9-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c01d9-208">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="c01d9-208">certificationAuthority</span></span>|<span data-ttu-id="c01d9-209">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-209">String</span></span>|<span data-ttu-id="c01d9-210">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c01d9-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c01d9-211">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="c01d9-211">certificationAuthorityName</span></span>|<span data-ttu-id="c01d9-212">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-212">String</span></span>|<span data-ttu-id="c01d9-213">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c01d9-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c01d9-214">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="c01d9-214">certificateTemplateName</span></span>|<span data-ttu-id="c01d9-215">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-215">String</span></span>|<span data-ttu-id="c01d9-216">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="c01d9-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c01d9-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c01d9-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c01d9-218">String</span><span class="sxs-lookup"><span data-stu-id="c01d9-218">String</span></span>|<span data-ttu-id="c01d9-219">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c01d9-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c01d9-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="c01d9-220">Response</span></span>
<span data-ttu-id="c01d9-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c01d9-221">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c01d9-222">Пример</span><span class="sxs-lookup"><span data-stu-id="c01d9-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="c01d9-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="c01d9-223">Request</span></span>
<span data-ttu-id="c01d9-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c01d9-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1738

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="c01d9-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="c01d9-225">Response</span></span>
<span data-ttu-id="c01d9-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c01d9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1910

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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



