---
title: Создание Андроиддевицеовнерсцепцертификатепрофиле
description: Создание нового объекта Андроиддевицеовнерсцепцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bf596fc28236bc1376423f45d78b5258bac16c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436144"
---
# <a name="create-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="485aa-103">Создание Андроиддевицеовнерсцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="485aa-103">Create androidDeviceOwnerScepCertificateProfile</span></span>

<span data-ttu-id="485aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="485aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="485aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="485aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="485aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="485aa-107">Создание нового объекта [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="485aa-107">Create a new [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="485aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="485aa-108">Prerequisites</span></span>
<span data-ttu-id="485aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485aa-111">Permission type</span></span>|<span data-ttu-id="485aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="485aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="485aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="485aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="485aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="485aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485aa-116">Not supported.</span></span>|
|<span data-ttu-id="485aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485aa-117">Application</span></span>|<span data-ttu-id="485aa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485aa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="485aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="485aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="485aa-120">Request headers</span></span>
|<span data-ttu-id="485aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="485aa-121">Header</span></span>|<span data-ttu-id="485aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="485aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="485aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="485aa-123">Authorization</span></span>|<span data-ttu-id="485aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="485aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="485aa-125">Accept</span></span>|<span data-ttu-id="485aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="485aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="485aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="485aa-127">Request body</span></span>
<span data-ttu-id="485aa-128">В тексте запроса добавьте представление объекта Андроиддевицеовнерсцепцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="485aa-128">In the request body, supply a JSON representation for the androidDeviceOwnerScepCertificateProfile object.</span></span>

<span data-ttu-id="485aa-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерсцепцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="485aa-129">The following table shows the properties that are required when you create the androidDeviceOwnerScepCertificateProfile.</span></span>

|<span data-ttu-id="485aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="485aa-130">Property</span></span>|<span data-ttu-id="485aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="485aa-131">Type</span></span>|<span data-ttu-id="485aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="485aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="485aa-133">id</span><span class="sxs-lookup"><span data-stu-id="485aa-133">id</span></span>|<span data-ttu-id="485aa-134">String</span><span class="sxs-lookup"><span data-stu-id="485aa-134">String</span></span>|<span data-ttu-id="485aa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="485aa-135">Key of the entity.</span></span> <span data-ttu-id="485aa-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="485aa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="485aa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="485aa-138">DateTimeOffset</span></span>|<span data-ttu-id="485aa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="485aa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="485aa-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="485aa-141">roleScopeTagIds</span></span>|<span data-ttu-id="485aa-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="485aa-142">String collection</span></span>|<span data-ttu-id="485aa-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="485aa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="485aa-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="485aa-145">supportsScopeTags</span></span>|<span data-ttu-id="485aa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="485aa-146">Boolean</span></span>|<span data-ttu-id="485aa-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="485aa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="485aa-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="485aa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="485aa-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="485aa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="485aa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="485aa-150">This property is read-only.</span></span> <span data-ttu-id="485aa-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="485aa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="485aa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="485aa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="485aa-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="485aa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="485aa-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="485aa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="485aa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="485aa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="485aa-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="485aa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="485aa-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="485aa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="485aa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="485aa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="485aa-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="485aa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="485aa-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="485aa-164">createdDateTime</span></span>|<span data-ttu-id="485aa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="485aa-165">DateTimeOffset</span></span>|<span data-ttu-id="485aa-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="485aa-166">DateTime the object was created.</span></span> <span data-ttu-id="485aa-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-168">description</span><span class="sxs-lookup"><span data-stu-id="485aa-168">description</span></span>|<span data-ttu-id="485aa-169">String</span><span class="sxs-lookup"><span data-stu-id="485aa-169">String</span></span>|<span data-ttu-id="485aa-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="485aa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="485aa-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="485aa-172">displayName</span></span>|<span data-ttu-id="485aa-173">Строка</span><span class="sxs-lookup"><span data-stu-id="485aa-173">String</span></span>|<span data-ttu-id="485aa-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="485aa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="485aa-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-176">version</span><span class="sxs-lookup"><span data-stu-id="485aa-176">version</span></span>|<span data-ttu-id="485aa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="485aa-177">Int32</span></span>|<span data-ttu-id="485aa-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="485aa-178">Version of the device configuration.</span></span> <span data-ttu-id="485aa-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="485aa-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="485aa-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="485aa-181">Int32</span><span class="sxs-lookup"><span data-stu-id="485aa-181">Int32</span></span>|<span data-ttu-id="485aa-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="485aa-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="485aa-183">Допустимые значения — от 1 до 99, наследуемые от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="485aa-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="485aa-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="485aa-184">subjectNameFormat</span></span>|[<span data-ttu-id="485aa-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="485aa-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="485aa-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="485aa-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="485aa-187">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="485aa-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="485aa-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="485aa-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="485aa-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="485aa-190">Int32</span><span class="sxs-lookup"><span data-stu-id="485aa-190">Int32</span></span>|<span data-ttu-id="485aa-191">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="485aa-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="485aa-192">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="485aa-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="485aa-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="485aa-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="485aa-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="485aa-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="485aa-195">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="485aa-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="485aa-196">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="485aa-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="485aa-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="485aa-198">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="485aa-198">extendedKeyUsages</span></span>|<span data-ttu-id="485aa-199">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="485aa-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="485aa-200">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="485aa-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="485aa-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="485aa-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="485aa-202">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="485aa-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="485aa-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="485aa-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="485aa-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="485aa-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="485aa-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="485aa-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="485aa-206">Наследуется от [андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="485aa-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="485aa-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="485aa-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="485aa-208">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="485aa-208">scepServerUrls</span></span>|<span data-ttu-id="485aa-209">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="485aa-209">String collection</span></span>|<span data-ttu-id="485aa-210">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="485aa-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="485aa-211">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="485aa-211">subjectNameFormatString</span></span>|<span data-ttu-id="485aa-212">String</span><span class="sxs-lookup"><span data-stu-id="485aa-212">String</span></span>|<span data-ttu-id="485aa-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="485aa-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="485aa-214">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="485aa-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="485aa-215">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="485aa-215">keyUsage</span></span>|[<span data-ttu-id="485aa-216">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="485aa-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="485aa-217">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="485aa-217">SCEP Key Usage.</span></span> <span data-ttu-id="485aa-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="485aa-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="485aa-219">keySize</span><span class="sxs-lookup"><span data-stu-id="485aa-219">keySize</span></span>|[<span data-ttu-id="485aa-220">keySize</span><span class="sxs-lookup"><span data-stu-id="485aa-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="485aa-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="485aa-221">SCEP Key Size.</span></span> <span data-ttu-id="485aa-222">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="485aa-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="485aa-223">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="485aa-223">hashAlgorithm</span></span>|[<span data-ttu-id="485aa-224">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="485aa-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="485aa-225">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="485aa-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="485aa-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="485aa-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="485aa-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="485aa-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="485aa-228">String</span><span class="sxs-lookup"><span data-stu-id="485aa-228">String</span></span>|<span data-ttu-id="485aa-229">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="485aa-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="485aa-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="485aa-230">certificateStore</span></span>|[<span data-ttu-id="485aa-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="485aa-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="485aa-232">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="485aa-232">Target store certificate.</span></span> <span data-ttu-id="485aa-233">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="485aa-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="485aa-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="485aa-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="485aa-235">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="485aa-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="485aa-236">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="485aa-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="485aa-237">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="485aa-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="485aa-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="485aa-238">Response</span></span>
<span data-ttu-id="485aa-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="485aa-239">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485aa-240">Пример</span><span class="sxs-lookup"><span data-stu-id="485aa-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="485aa-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="485aa-241">Request</span></span>
<span data-ttu-id="485aa-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="485aa-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="485aa-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="485aa-243">Response</span></span>
<span data-ttu-id="485aa-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="485aa-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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



