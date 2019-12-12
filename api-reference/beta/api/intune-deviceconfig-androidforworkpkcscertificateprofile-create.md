---
title: Создание androidForWorkPkcsCertificateProfile
description: Создание нового объекта androidForWorkPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46362836469fa52620362a655fffbab4765ae6ef
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954757"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="607b2-103">Создание androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="607b2-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="607b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="607b2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="607b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="607b2-106">Создание нового объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="607b2-106">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="607b2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="607b2-107">Prerequisites</span></span>
<span data-ttu-id="607b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="607b2-110">Permission type</span></span>|<span data-ttu-id="607b2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="607b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="607b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="607b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="607b2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607b2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="607b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="607b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="607b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607b2-115">Not supported.</span></span>|
|<span data-ttu-id="607b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="607b2-116">Application</span></span>|<span data-ttu-id="607b2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607b2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="607b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="607b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="607b2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="607b2-119">Request headers</span></span>
|<span data-ttu-id="607b2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="607b2-120">Header</span></span>|<span data-ttu-id="607b2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="607b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="607b2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="607b2-122">Authorization</span></span>|<span data-ttu-id="607b2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="607b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="607b2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="607b2-124">Accept</span></span>|<span data-ttu-id="607b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="607b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="607b2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="607b2-126">Request body</span></span>
<span data-ttu-id="607b2-127">В тексте запроса добавьте представление объекта androidForWorkPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="607b2-127">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="607b2-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="607b2-128">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="607b2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="607b2-129">Property</span></span>|<span data-ttu-id="607b2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="607b2-130">Type</span></span>|<span data-ttu-id="607b2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="607b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="607b2-132">id</span><span class="sxs-lookup"><span data-stu-id="607b2-132">id</span></span>|<span data-ttu-id="607b2-133">String</span><span class="sxs-lookup"><span data-stu-id="607b2-133">String</span></span>|<span data-ttu-id="607b2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="607b2-134">Key of the entity.</span></span> <span data-ttu-id="607b2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="607b2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="607b2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="607b2-137">DateTimeOffset</span></span>|<span data-ttu-id="607b2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="607b2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="607b2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="607b2-140">roleScopeTagIds</span></span>|<span data-ttu-id="607b2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="607b2-141">String collection</span></span>|<span data-ttu-id="607b2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="607b2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="607b2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="607b2-144">supportsScopeTags</span></span>|<span data-ttu-id="607b2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="607b2-145">Boolean</span></span>|<span data-ttu-id="607b2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="607b2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="607b2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="607b2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="607b2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="607b2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="607b2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="607b2-149">This property is read-only.</span></span> <span data-ttu-id="607b2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="607b2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="607b2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="607b2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="607b2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="607b2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="607b2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="607b2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="607b2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="607b2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="607b2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="607b2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="607b2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="607b2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="607b2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="607b2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="607b2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="607b2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="607b2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="607b2-163">createdDateTime</span></span>|<span data-ttu-id="607b2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="607b2-164">DateTimeOffset</span></span>|<span data-ttu-id="607b2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="607b2-165">DateTime the object was created.</span></span> <span data-ttu-id="607b2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-167">description</span><span class="sxs-lookup"><span data-stu-id="607b2-167">description</span></span>|<span data-ttu-id="607b2-168">String</span><span class="sxs-lookup"><span data-stu-id="607b2-168">String</span></span>|<span data-ttu-id="607b2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="607b2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="607b2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="607b2-171">displayName</span></span>|<span data-ttu-id="607b2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="607b2-172">String</span></span>|<span data-ttu-id="607b2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="607b2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="607b2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-175">version</span><span class="sxs-lookup"><span data-stu-id="607b2-175">version</span></span>|<span data-ttu-id="607b2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="607b2-176">Int32</span></span>|<span data-ttu-id="607b2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="607b2-177">Version of the device configuration.</span></span> <span data-ttu-id="607b2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="607b2-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="607b2-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="607b2-180">Int32</span><span class="sxs-lookup"><span data-stu-id="607b2-180">Int32</span></span>|<span data-ttu-id="607b2-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="607b2-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="607b2-182">Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="607b2-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="607b2-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="607b2-183">subjectNameFormat</span></span>|[<span data-ttu-id="607b2-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="607b2-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="607b2-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="607b2-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="607b2-186">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="607b2-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="607b2-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="607b2-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="607b2-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="607b2-189">Int32</span><span class="sxs-lookup"><span data-stu-id="607b2-189">Int32</span></span>|<span data-ttu-id="607b2-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="607b2-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="607b2-191">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="607b2-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="607b2-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="607b2-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="607b2-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="607b2-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="607b2-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="607b2-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="607b2-195">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="607b2-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="607b2-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="607b2-197">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="607b2-197">extendedKeyUsages</span></span>|<span data-ttu-id="607b2-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="607b2-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="607b2-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="607b2-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="607b2-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="607b2-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="607b2-201">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="607b2-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="607b2-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="607b2-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="607b2-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="607b2-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="607b2-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="607b2-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="607b2-205">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="607b2-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="607b2-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="607b2-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="607b2-207">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="607b2-207">certificationAuthority</span></span>|<span data-ttu-id="607b2-208">Строка</span><span class="sxs-lookup"><span data-stu-id="607b2-208">String</span></span>|<span data-ttu-id="607b2-209">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="607b2-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="607b2-210">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="607b2-210">certificationAuthorityName</span></span>|<span data-ttu-id="607b2-211">Строка</span><span class="sxs-lookup"><span data-stu-id="607b2-211">String</span></span>|<span data-ttu-id="607b2-212">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="607b2-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="607b2-213">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="607b2-213">certificateTemplateName</span></span>|<span data-ttu-id="607b2-214">Строка</span><span class="sxs-lookup"><span data-stu-id="607b2-214">String</span></span>|<span data-ttu-id="607b2-215">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="607b2-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="607b2-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="607b2-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="607b2-217">Строка</span><span class="sxs-lookup"><span data-stu-id="607b2-217">String</span></span>|<span data-ttu-id="607b2-218">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="607b2-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="607b2-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="607b2-219">Response</span></span>
<span data-ttu-id="607b2-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="607b2-220">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607b2-221">Пример</span><span class="sxs-lookup"><span data-stu-id="607b2-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="607b2-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="607b2-222">Request</span></span>
<span data-ttu-id="607b2-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="607b2-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="607b2-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="607b2-224">Response</span></span>
<span data-ttu-id="607b2-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="607b2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





