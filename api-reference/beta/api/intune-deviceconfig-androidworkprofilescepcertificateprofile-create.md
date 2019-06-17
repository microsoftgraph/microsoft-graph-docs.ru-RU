---
title: Создание Андроидворкпрофилесцепцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилесцепцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8949b22e88456379d673d157fd552cd37b07f70
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969101"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="c3fe1-103">Создание Андроидворкпрофилесцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="c3fe1-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="c3fe1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3fe1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3fe1-106">Создание нового объекта [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c3fe1-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3fe1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3fe1-107">Prerequisites</span></span>
<span data-ttu-id="c3fe1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3fe1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3fe1-110">Permission type</span></span>|<span data-ttu-id="c3fe1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3fe1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3fe1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3fe1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3fe1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3fe1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-115">Not supported.</span></span>|
|<span data-ttu-id="c3fe1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3fe1-116">Application</span></span>|<span data-ttu-id="c3fe1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3fe1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3fe1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3fe1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3fe1-119">Request headers</span></span>
|<span data-ttu-id="c3fe1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3fe1-120">Header</span></span>|<span data-ttu-id="c3fe1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c3fe1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3fe1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3fe1-122">Authorization</span></span>|<span data-ttu-id="c3fe1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3fe1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c3fe1-124">Accept</span></span>|<span data-ttu-id="c3fe1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3fe1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3fe1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3fe1-126">Request body</span></span>
<span data-ttu-id="c3fe1-127">В тексте запроса добавьте представление объекта Андроидворкпрофилесцепцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="c3fe1-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилесцепцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="c3fe1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3fe1-129">Property</span></span>|<span data-ttu-id="c3fe1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3fe1-130">Type</span></span>|<span data-ttu-id="c3fe1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3fe1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3fe1-132">id</span><span class="sxs-lookup"><span data-stu-id="c3fe1-132">id</span></span>|<span data-ttu-id="c3fe1-133">String</span><span class="sxs-lookup"><span data-stu-id="c3fe1-133">String</span></span>|<span data-ttu-id="c3fe1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-134">Key of the entity.</span></span> <span data-ttu-id="c3fe1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3fe1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c3fe1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3fe1-137">DateTimeOffset</span></span>|<span data-ttu-id="c3fe1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c3fe1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3fe1-140">roleScopeTagIds</span></span>|<span data-ttu-id="c3fe1-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3fe1-141">String collection</span></span>|<span data-ttu-id="c3fe1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3fe1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c3fe1-144">supportsScopeTags</span></span>|<span data-ttu-id="c3fe1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3fe1-145">Boolean</span></span>|<span data-ttu-id="c3fe1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3fe1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3fe1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3fe1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-149">This property is read-only.</span></span> <span data-ttu-id="c3fe1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3fe1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c3fe1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3fe1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c3fe1-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c3fe1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3fe1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c3fe1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3fe1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c3fe1-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c3fe1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c3fe1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c3fe1-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c3fe1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c3fe1-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c3fe1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3fe1-163">createdDateTime</span></span>|<span data-ttu-id="c3fe1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3fe1-164">DateTimeOffset</span></span>|<span data-ttu-id="c3fe1-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-165">DateTime the object was created.</span></span> <span data-ttu-id="c3fe1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-167">description</span><span class="sxs-lookup"><span data-stu-id="c3fe1-167">description</span></span>|<span data-ttu-id="c3fe1-168">String</span><span class="sxs-lookup"><span data-stu-id="c3fe1-168">String</span></span>|<span data-ttu-id="c3fe1-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3fe1-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c3fe1-171">displayName</span></span>|<span data-ttu-id="c3fe1-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c3fe1-172">String</span></span>|<span data-ttu-id="c3fe1-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3fe1-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-175">version</span><span class="sxs-lookup"><span data-stu-id="c3fe1-175">version</span></span>|<span data-ttu-id="c3fe1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c3fe1-176">Int32</span></span>|<span data-ttu-id="c3fe1-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-177">Version of the device configuration.</span></span> <span data-ttu-id="c3fe1-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3fe1-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c3fe1-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c3fe1-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c3fe1-180">Int32</span></span>|<span data-ttu-id="c3fe1-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c3fe1-182">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3fe1-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c3fe1-183">subjectNameFormat</span></span>|[<span data-ttu-id="c3fe1-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c3fe1-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c3fe1-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="c3fe1-186">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c3fe1-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c3fe1-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c3fe1-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c3fe1-189">Int32</span><span class="sxs-lookup"><span data-stu-id="c3fe1-189">Int32</span></span>|<span data-ttu-id="c3fe1-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c3fe1-191">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3fe1-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c3fe1-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c3fe1-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c3fe1-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c3fe1-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c3fe1-195">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c3fe1-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c3fe1-197">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c3fe1-197">extendedKeyUsages</span></span>|<span data-ttu-id="c3fe1-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c3fe1-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c3fe1-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c3fe1-201">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c3fe1-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c3fe1-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c3fe1-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c3fe1-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c3fe1-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c3fe1-205">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c3fe1-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c3fe1-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c3fe1-207">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="c3fe1-207">scepServerUrls</span></span>|<span data-ttu-id="c3fe1-208">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3fe1-208">String collection</span></span>|<span data-ttu-id="c3fe1-209">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="c3fe1-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="c3fe1-210">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="c3fe1-210">subjectNameFormatString</span></span>|<span data-ttu-id="c3fe1-211">String</span><span class="sxs-lookup"><span data-stu-id="c3fe1-211">String</span></span>|<span data-ttu-id="c3fe1-212">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c3fe1-213">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="c3fe1-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c3fe1-214">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="c3fe1-214">keyUsage</span></span>|[<span data-ttu-id="c3fe1-215">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="c3fe1-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c3fe1-216">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-216">SCEP Key Usage.</span></span> <span data-ttu-id="c3fe1-217">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c3fe1-218">keySize</span><span class="sxs-lookup"><span data-stu-id="c3fe1-218">keySize</span></span>|[<span data-ttu-id="c3fe1-219">keySize</span><span class="sxs-lookup"><span data-stu-id="c3fe1-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c3fe1-220">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-220">SCEP Key Size.</span></span> <span data-ttu-id="c3fe1-221">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c3fe1-222">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="c3fe1-222">hashAlgorithm</span></span>|[<span data-ttu-id="c3fe1-223">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="c3fe1-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c3fe1-224">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c3fe1-225">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c3fe1-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c3fe1-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c3fe1-227">String</span><span class="sxs-lookup"><span data-stu-id="c3fe1-227">String</span></span>|<span data-ttu-id="c3fe1-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c3fe1-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c3fe1-229">certificateStore</span></span>|[<span data-ttu-id="c3fe1-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c3fe1-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="c3fe1-231">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-231">Target store certificate.</span></span> <span data-ttu-id="c3fe1-232">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c3fe1-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c3fe1-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c3fe1-234">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="c3fe1-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c3fe1-235">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="c3fe1-236">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c3fe1-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3fe1-237">Response</span></span>
<span data-ttu-id="c3fe1-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилесцепцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-238">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3fe1-239">Пример</span><span class="sxs-lookup"><span data-stu-id="c3fe1-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3fe1-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3fe1-240">Request</span></span>
<span data-ttu-id="c3fe1-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3fe1-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3fe1-242">Response</span></span>
<span data-ttu-id="c3fe1-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3fe1-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





