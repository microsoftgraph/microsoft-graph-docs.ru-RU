---
title: Создание androidForWorkPkcsCertificateProfile
description: Создайте новый объект AndroidForWorkPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f95f36d6eed71e7b38bdff3e443e71ed3533f607
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142599"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="66b82-103">Создание androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="66b82-103">Create androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="66b82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66b82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66b82-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66b82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66b82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66b82-107">Создайте новый [объект AndroidForWorkPkcsCertificateProfile.](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="66b82-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66b82-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="66b82-108">Prerequisites</span></span>
<span data-ttu-id="66b82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66b82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66b82-111">Permission type</span></span>|<span data-ttu-id="66b82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66b82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66b82-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66b82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66b82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66b82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66b82-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66b82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66b82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b82-116">Not supported.</span></span>|
|<span data-ttu-id="66b82-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="66b82-117">Application</span></span>|<span data-ttu-id="66b82-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66b82-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66b82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66b82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66b82-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66b82-120">Request headers</span></span>
|<span data-ttu-id="66b82-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66b82-121">Header</span></span>|<span data-ttu-id="66b82-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66b82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66b82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b82-123">Authorization</span></span>|<span data-ttu-id="66b82-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66b82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66b82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66b82-125">Accept</span></span>|<span data-ttu-id="66b82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66b82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66b82-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66b82-127">Request body</span></span>
<span data-ttu-id="66b82-128">В теле запроса поставляем представление JSON для объекта AndroidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="66b82-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="66b82-129">В следующей таблице показаны свойства, необходимые при создании androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="66b82-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="66b82-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66b82-130">Property</span></span>|<span data-ttu-id="66b82-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66b82-131">Type</span></span>|<span data-ttu-id="66b82-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66b82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b82-133">id</span><span class="sxs-lookup"><span data-stu-id="66b82-133">id</span></span>|<span data-ttu-id="66b82-134">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-134">String</span></span>|<span data-ttu-id="66b82-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66b82-135">Key of the entity.</span></span> <span data-ttu-id="66b82-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66b82-137">lastModifiedDateTime</span></span>|<span data-ttu-id="66b82-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66b82-138">DateTimeOffset</span></span>|<span data-ttu-id="66b82-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="66b82-139">DateTime the object was last modified.</span></span> <span data-ttu-id="66b82-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66b82-141">roleScopeTagIds</span></span>|<span data-ttu-id="66b82-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66b82-142">String collection</span></span>|<span data-ttu-id="66b82-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="66b82-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66b82-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66b82-145">supportsScopeTags</span></span>|<span data-ttu-id="66b82-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="66b82-146">Boolean</span></span>|<span data-ttu-id="66b82-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="66b82-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66b82-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="66b82-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66b82-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="66b82-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66b82-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66b82-150">This property is read-only.</span></span> <span data-ttu-id="66b82-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66b82-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="66b82-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66b82-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="66b82-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66b82-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="66b82-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66b82-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="66b82-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66b82-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="66b82-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66b82-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="66b82-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="66b82-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="66b82-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="66b82-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="66b82-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66b82-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="66b82-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66b82-164">createdDateTime</span></span>|<span data-ttu-id="66b82-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66b82-165">DateTimeOffset</span></span>|<span data-ttu-id="66b82-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="66b82-166">DateTime the object was created.</span></span> <span data-ttu-id="66b82-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-168">description</span><span class="sxs-lookup"><span data-stu-id="66b82-168">description</span></span>|<span data-ttu-id="66b82-169">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-169">String</span></span>|<span data-ttu-id="66b82-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66b82-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66b82-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-172">displayName</span><span class="sxs-lookup"><span data-stu-id="66b82-172">displayName</span></span>|<span data-ttu-id="66b82-173">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-173">String</span></span>|<span data-ttu-id="66b82-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66b82-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66b82-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-176">version</span><span class="sxs-lookup"><span data-stu-id="66b82-176">version</span></span>|<span data-ttu-id="66b82-177">Int32</span><span class="sxs-lookup"><span data-stu-id="66b82-177">Int32</span></span>|<span data-ttu-id="66b82-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66b82-178">Version of the device configuration.</span></span> <span data-ttu-id="66b82-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66b82-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="66b82-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="66b82-181">Int32</span><span class="sxs-lookup"><span data-stu-id="66b82-181">Int32</span></span>|<span data-ttu-id="66b82-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="66b82-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="66b82-183">Допустимые значения от 1 до 99, унаследованные от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66b82-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="66b82-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66b82-184">subjectNameFormat</span></span>|[<span data-ttu-id="66b82-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66b82-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="66b82-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="66b82-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="66b82-187">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="66b82-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="66b82-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="66b82-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="66b82-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="66b82-190">Int32</span><span class="sxs-lookup"><span data-stu-id="66b82-190">Int32</span></span>|<span data-ttu-id="66b82-191">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="66b82-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="66b82-192">Унаследованный от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66b82-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="66b82-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="66b82-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="66b82-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="66b82-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="66b82-195">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="66b82-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="66b82-196">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="66b82-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="66b82-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="66b82-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="66b82-198">extendedKeyUsages</span></span>|<span data-ttu-id="66b82-199">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="66b82-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="66b82-200">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="66b82-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="66b82-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="66b82-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="66b82-202">Унаследованный от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66b82-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="66b82-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="66b82-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="66b82-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="66b82-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="66b82-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="66b82-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="66b82-206">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="66b82-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="66b82-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="66b82-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="66b82-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="66b82-208">certificationAuthority</span></span>|<span data-ttu-id="66b82-209">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-209">String</span></span>|<span data-ttu-id="66b82-210">Сертификационный орган PKCS</span><span class="sxs-lookup"><span data-stu-id="66b82-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="66b82-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="66b82-211">certificationAuthorityName</span></span>|<span data-ttu-id="66b82-212">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-212">String</span></span>|<span data-ttu-id="66b82-213">Имя органа сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="66b82-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="66b82-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="66b82-214">certificateTemplateName</span></span>|<span data-ttu-id="66b82-215">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-215">String</span></span>|<span data-ttu-id="66b82-216">Имя шаблона шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="66b82-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="66b82-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="66b82-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="66b82-218">Строка</span><span class="sxs-lookup"><span data-stu-id="66b82-218">String</span></span>|<span data-ttu-id="66b82-219">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="66b82-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="66b82-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b82-220">Response</span></span>
<span data-ttu-id="66b82-221">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidForWorkPkkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="66b82-221">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66b82-222">Пример</span><span class="sxs-lookup"><span data-stu-id="66b82-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="66b82-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="66b82-223">Request</span></span>
<span data-ttu-id="66b82-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66b82-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66b82-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b82-225">Response</span></span>
<span data-ttu-id="66b82-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66b82-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




