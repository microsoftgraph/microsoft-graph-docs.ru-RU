---
title: Создание androidForWorkPkcsCertificateProfile
description: Создание нового объекта androidForWorkPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c890ccdfb366dbac1ca5eb8011fc142067afd9a5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970585"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="c1ab3-103">Создание androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c1ab3-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="c1ab3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1ab3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ab3-106">Создание нового объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c1ab3-106">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ab3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1ab3-107">Prerequisites</span></span>
<span data-ttu-id="c1ab3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ab3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1ab3-110">Permission type</span></span>|<span data-ttu-id="c1ab3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ab3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ab3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ab3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1ab3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ab3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-115">Not supported.</span></span>|
|<span data-ttu-id="c1ab3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1ab3-116">Application</span></span>|<span data-ttu-id="c1ab3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ab3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1ab3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1ab3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1ab3-119">Request headers</span></span>
|<span data-ttu-id="c1ab3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1ab3-120">Header</span></span>|<span data-ttu-id="c1ab3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1ab3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ab3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1ab3-122">Authorization</span></span>|<span data-ttu-id="c1ab3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ab3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1ab3-124">Accept</span></span>|<span data-ttu-id="c1ab3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ab3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ab3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1ab3-126">Request body</span></span>
<span data-ttu-id="c1ab3-127">В тексте запроса добавьте представление объекта androidForWorkPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-127">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="c1ab3-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-128">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="c1ab3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1ab3-129">Property</span></span>|<span data-ttu-id="c1ab3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c1ab3-130">Type</span></span>|<span data-ttu-id="c1ab3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c1ab3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ab3-132">id</span><span class="sxs-lookup"><span data-stu-id="c1ab3-132">id</span></span>|<span data-ttu-id="c1ab3-133">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-133">String</span></span>|<span data-ttu-id="c1ab3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-134">Key of the entity.</span></span> <span data-ttu-id="c1ab3-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ab3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c1ab3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ab3-137">DateTimeOffset</span></span>|<span data-ttu-id="c1ab3-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c1ab3-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1ab3-140">roleScopeTagIds</span></span>|<span data-ttu-id="c1ab3-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c1ab3-141">String collection</span></span>|<span data-ttu-id="c1ab3-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1ab3-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c1ab3-144">supportsScopeTags</span></span>|<span data-ttu-id="c1ab3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1ab3-145">Boolean</span></span>|<span data-ttu-id="c1ab3-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1ab3-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1ab3-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1ab3-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-149">This property is read-only.</span></span> <span data-ttu-id="c1ab3-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1ab3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c1ab3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1ab3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c1ab3-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c1ab3-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1ab3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c1ab3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1ab3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c1ab3-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c1ab3-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c1ab3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c1ab3-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c1ab3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c1ab3-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c1ab3-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ab3-163">createdDateTime</span></span>|<span data-ttu-id="c1ab3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ab3-164">DateTimeOffset</span></span>|<span data-ttu-id="c1ab3-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-165">DateTime the object was created.</span></span> <span data-ttu-id="c1ab3-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-167">description</span><span class="sxs-lookup"><span data-stu-id="c1ab3-167">description</span></span>|<span data-ttu-id="c1ab3-168">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-168">String</span></span>|<span data-ttu-id="c1ab3-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1ab3-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ab3-171">displayName</span></span>|<span data-ttu-id="c1ab3-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c1ab3-172">String</span></span>|<span data-ttu-id="c1ab3-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1ab3-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-175">version</span><span class="sxs-lookup"><span data-stu-id="c1ab3-175">version</span></span>|<span data-ttu-id="c1ab3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c1ab3-176">Int32</span></span>|<span data-ttu-id="c1ab3-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-177">Version of the device configuration.</span></span> <span data-ttu-id="c1ab3-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1ab3-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c1ab3-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c1ab3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c1ab3-180">Int32</span></span>|<span data-ttu-id="c1ab3-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c1ab3-182">Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1ab3-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c1ab3-183">subjectNameFormat</span></span>|[<span data-ttu-id="c1ab3-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c1ab3-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c1ab3-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="c1ab3-186">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c1ab3-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c1ab3-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c1ab3-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c1ab3-189">Int32</span><span class="sxs-lookup"><span data-stu-id="c1ab3-189">Int32</span></span>|<span data-ttu-id="c1ab3-190">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c1ab3-191">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1ab3-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c1ab3-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c1ab3-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c1ab3-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c1ab3-194">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c1ab3-195">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c1ab3-196">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c1ab3-197">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c1ab3-197">extendedKeyUsages</span></span>|<span data-ttu-id="c1ab3-198">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c1ab3-199">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c1ab3-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c1ab3-201">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c1ab3-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c1ab3-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c1ab3-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c1ab3-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c1ab3-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c1ab3-204">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c1ab3-205">Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1ab3-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="c1ab3-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c1ab3-207">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="c1ab3-207">certificationAuthority</span></span>|<span data-ttu-id="c1ab3-208">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-208">String</span></span>|<span data-ttu-id="c1ab3-209">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c1ab3-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c1ab3-210">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="c1ab3-210">certificationAuthorityName</span></span>|<span data-ttu-id="c1ab3-211">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-211">String</span></span>|<span data-ttu-id="c1ab3-212">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c1ab3-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c1ab3-213">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="c1ab3-213">certificateTemplateName</span></span>|<span data-ttu-id="c1ab3-214">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-214">String</span></span>|<span data-ttu-id="c1ab3-215">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="c1ab3-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c1ab3-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c1ab3-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c1ab3-217">String</span><span class="sxs-lookup"><span data-stu-id="c1ab3-217">String</span></span>|<span data-ttu-id="c1ab3-218">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c1ab3-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ab3-219">Response</span></span>
<span data-ttu-id="c1ab3-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-220">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ab3-221">Пример</span><span class="sxs-lookup"><span data-stu-id="c1ab3-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ab3-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1ab3-222">Request</span></span>
<span data-ttu-id="c1ab3-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1ab3-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ab3-224">Response</span></span>
<span data-ttu-id="c1ab3-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1ab3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





