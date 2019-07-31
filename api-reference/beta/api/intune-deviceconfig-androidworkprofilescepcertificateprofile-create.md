---
title: Создание Андроидворкпрофилесцепцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилесцепцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7078d12f7fcb4f6afc4cdf2182304088df936aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950548"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="12d53-103">Создание Андроидворкпрофилесцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="12d53-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="12d53-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12d53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12d53-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12d53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d53-106">Создание нового объекта [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="12d53-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12d53-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12d53-107">Prerequisites</span></span>
<span data-ttu-id="12d53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d53-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12d53-110">Permission type</span></span>|<span data-ttu-id="12d53-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12d53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d53-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12d53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12d53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12d53-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12d53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12d53-115">Not supported.</span></span>|
|<span data-ttu-id="12d53-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12d53-116">Application</span></span>|<span data-ttu-id="12d53-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12d53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d53-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12d53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12d53-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12d53-119">Request headers</span></span>
|<span data-ttu-id="12d53-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12d53-120">Header</span></span>|<span data-ttu-id="12d53-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12d53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d53-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12d53-122">Authorization</span></span>|<span data-ttu-id="12d53-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12d53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12d53-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12d53-124">Accept</span></span>|<span data-ttu-id="12d53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12d53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d53-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12d53-126">Request body</span></span>
<span data-ttu-id="12d53-127">В тексте запроса добавьте представление объекта Андроидворкпрофилесцепцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12d53-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="12d53-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилесцепцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="12d53-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="12d53-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="12d53-129">Property</span></span>|<span data-ttu-id="12d53-130">Тип</span><span class="sxs-lookup"><span data-stu-id="12d53-130">Type</span></span>|<span data-ttu-id="12d53-131">Описание</span><span class="sxs-lookup"><span data-stu-id="12d53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d53-132">id</span><span class="sxs-lookup"><span data-stu-id="12d53-132">id</span></span>|<span data-ttu-id="12d53-133">String</span><span class="sxs-lookup"><span data-stu-id="12d53-133">String</span></span>|<span data-ttu-id="12d53-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12d53-134">Key of the entity.</span></span> <span data-ttu-id="12d53-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12d53-136">lastModifiedDateTime</span></span>|<span data-ttu-id="12d53-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d53-137">DateTimeOffset</span></span>|<span data-ttu-id="12d53-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="12d53-138">DateTime the object was last modified.</span></span> <span data-ttu-id="12d53-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12d53-140">roleScopeTagIds</span></span>|<span data-ttu-id="12d53-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12d53-141">String collection</span></span>|<span data-ttu-id="12d53-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="12d53-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12d53-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="12d53-144">supportsScopeTags</span></span>|<span data-ttu-id="12d53-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d53-145">Boolean</span></span>|<span data-ttu-id="12d53-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="12d53-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12d53-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="12d53-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12d53-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="12d53-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12d53-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12d53-149">This property is read-only.</span></span> <span data-ttu-id="12d53-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12d53-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12d53-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12d53-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12d53-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12d53-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12d53-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12d53-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12d53-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12d53-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12d53-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12d53-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12d53-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="12d53-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12d53-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="12d53-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12d53-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12d53-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12d53-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12d53-163">createdDateTime</span></span>|<span data-ttu-id="12d53-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d53-164">DateTimeOffset</span></span>|<span data-ttu-id="12d53-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="12d53-165">DateTime the object was created.</span></span> <span data-ttu-id="12d53-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-167">description</span><span class="sxs-lookup"><span data-stu-id="12d53-167">description</span></span>|<span data-ttu-id="12d53-168">String</span><span class="sxs-lookup"><span data-stu-id="12d53-168">String</span></span>|<span data-ttu-id="12d53-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12d53-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12d53-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-171">displayName</span><span class="sxs-lookup"><span data-stu-id="12d53-171">displayName</span></span>|<span data-ttu-id="12d53-172">Строка</span><span class="sxs-lookup"><span data-stu-id="12d53-172">String</span></span>|<span data-ttu-id="12d53-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12d53-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12d53-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-175">version</span><span class="sxs-lookup"><span data-stu-id="12d53-175">version</span></span>|<span data-ttu-id="12d53-176">Int32</span><span class="sxs-lookup"><span data-stu-id="12d53-176">Int32</span></span>|<span data-ttu-id="12d53-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12d53-177">Version of the device configuration.</span></span> <span data-ttu-id="12d53-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12d53-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="12d53-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="12d53-180">Int32</span><span class="sxs-lookup"><span data-stu-id="12d53-180">Int32</span></span>|<span data-ttu-id="12d53-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="12d53-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="12d53-182">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="12d53-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="12d53-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="12d53-183">subjectNameFormat</span></span>|[<span data-ttu-id="12d53-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="12d53-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="12d53-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="12d53-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="12d53-186">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="12d53-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="12d53-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="12d53-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="12d53-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="12d53-189">Int32</span><span class="sxs-lookup"><span data-stu-id="12d53-189">Int32</span></span>|<span data-ttu-id="12d53-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="12d53-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="12d53-191">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="12d53-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="12d53-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="12d53-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="12d53-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="12d53-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="12d53-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="12d53-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="12d53-195">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="12d53-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="12d53-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="12d53-197">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="12d53-197">extendedKeyUsages</span></span>|<span data-ttu-id="12d53-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="12d53-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="12d53-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="12d53-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="12d53-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="12d53-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="12d53-201">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="12d53-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="12d53-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="12d53-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="12d53-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="12d53-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="12d53-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="12d53-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="12d53-205">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="12d53-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="12d53-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="12d53-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="12d53-207">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="12d53-207">scepServerUrls</span></span>|<span data-ttu-id="12d53-208">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12d53-208">String collection</span></span>|<span data-ttu-id="12d53-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="12d53-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="12d53-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="12d53-210">subjectNameFormatString</span></span>|<span data-ttu-id="12d53-211">String</span><span class="sxs-lookup"><span data-stu-id="12d53-211">String</span></span>|<span data-ttu-id="12d53-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="12d53-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="12d53-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="12d53-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="12d53-214">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="12d53-214">keyUsage</span></span>|[<span data-ttu-id="12d53-215">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="12d53-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="12d53-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="12d53-216">SCEP Key Usage.</span></span> <span data-ttu-id="12d53-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="12d53-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="12d53-218">keySize</span><span class="sxs-lookup"><span data-stu-id="12d53-218">keySize</span></span>|[<span data-ttu-id="12d53-219">keySize</span><span class="sxs-lookup"><span data-stu-id="12d53-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="12d53-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="12d53-220">SCEP Key Size.</span></span> <span data-ttu-id="12d53-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="12d53-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="12d53-222">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="12d53-222">hashAlgorithm</span></span>|[<span data-ttu-id="12d53-223">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="12d53-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="12d53-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="12d53-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="12d53-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="12d53-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="12d53-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="12d53-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="12d53-227">String</span><span class="sxs-lookup"><span data-stu-id="12d53-227">String</span></span>|<span data-ttu-id="12d53-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="12d53-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="12d53-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="12d53-229">certificateStore</span></span>|[<span data-ttu-id="12d53-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="12d53-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="12d53-231">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="12d53-231">Target store certificate.</span></span> <span data-ttu-id="12d53-232">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="12d53-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="12d53-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="12d53-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="12d53-234">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="12d53-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="12d53-235">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="12d53-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="12d53-236">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="12d53-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="12d53-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="12d53-237">Response</span></span>
<span data-ttu-id="12d53-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12d53-238">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d53-239">Пример</span><span class="sxs-lookup"><span data-stu-id="12d53-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="12d53-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="12d53-240">Request</span></span>
<span data-ttu-id="12d53-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12d53-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12d53-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="12d53-242">Response</span></span>
<span data-ttu-id="12d53-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12d53-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





