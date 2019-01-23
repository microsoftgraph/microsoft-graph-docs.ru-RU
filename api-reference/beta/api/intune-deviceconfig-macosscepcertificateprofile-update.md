---
title: Обновление macOSScepCertificateProfile
description: Обновление свойства объекта macOSScepCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 547a4468015a68bcbdb8bbfe13839f98edd6d9d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412207"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="34410-103">Обновление macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="34410-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="34410-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34410-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34410-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34410-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34410-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34410-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34410-107">Обновление свойства объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="34410-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34410-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="34410-108">Prerequisites</span></span>
<span data-ttu-id="34410-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34410-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34410-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34410-111">Permission type</span></span>|<span data-ttu-id="34410-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34410-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34410-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34410-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34410-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34410-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34410-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34410-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34410-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34410-116">Not supported.</span></span>|
|<span data-ttu-id="34410-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34410-117">Application</span></span>|<span data-ttu-id="34410-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34410-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34410-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34410-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34410-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34410-120">Request headers</span></span>
|<span data-ttu-id="34410-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34410-121">Header</span></span>|<span data-ttu-id="34410-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34410-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34410-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34410-123">Authorization</span></span>|<span data-ttu-id="34410-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34410-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34410-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34410-125">Accept</span></span>|<span data-ttu-id="34410-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34410-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34410-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34410-127">Request body</span></span>
<span data-ttu-id="34410-128">В тексте запроса укажите представление JSON для объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="34410-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="34410-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="34410-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="34410-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="34410-130">Property</span></span>|<span data-ttu-id="34410-131">Тип</span><span class="sxs-lookup"><span data-stu-id="34410-131">Type</span></span>|<span data-ttu-id="34410-132">Описание</span><span class="sxs-lookup"><span data-stu-id="34410-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34410-133">id</span><span class="sxs-lookup"><span data-stu-id="34410-133">id</span></span>|<span data-ttu-id="34410-134">String</span><span class="sxs-lookup"><span data-stu-id="34410-134">String</span></span>|<span data-ttu-id="34410-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34410-135">Key of the entity.</span></span> <span data-ttu-id="34410-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34410-137">lastModifiedDateTime</span></span>|<span data-ttu-id="34410-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34410-138">DateTimeOffset</span></span>|<span data-ttu-id="34410-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="34410-139">DateTime the object was last modified.</span></span> <span data-ttu-id="34410-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34410-141">roleScopeTagIds</span></span>|<span data-ttu-id="34410-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34410-142">String collection</span></span>|<span data-ttu-id="34410-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="34410-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34410-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34410-145">supportsScopeTags</span></span>|<span data-ttu-id="34410-146">Логический</span><span class="sxs-lookup"><span data-stu-id="34410-146">Boolean</span></span>|<span data-ttu-id="34410-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="34410-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34410-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="34410-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34410-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="34410-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34410-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34410-150">This property is read-only.</span></span> <span data-ttu-id="34410-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34410-152">createdDateTime</span></span>|<span data-ttu-id="34410-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34410-153">DateTimeOffset</span></span>|<span data-ttu-id="34410-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="34410-154">DateTime the object was created.</span></span> <span data-ttu-id="34410-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-156">description</span><span class="sxs-lookup"><span data-stu-id="34410-156">description</span></span>|<span data-ttu-id="34410-157">String</span><span class="sxs-lookup"><span data-stu-id="34410-157">String</span></span>|<span data-ttu-id="34410-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34410-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34410-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-160">displayName</span><span class="sxs-lookup"><span data-stu-id="34410-160">displayName</span></span>|<span data-ttu-id="34410-161">String</span><span class="sxs-lookup"><span data-stu-id="34410-161">String</span></span>|<span data-ttu-id="34410-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34410-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34410-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-164">version</span><span class="sxs-lookup"><span data-stu-id="34410-164">version</span></span>|<span data-ttu-id="34410-165">Int32</span><span class="sxs-lookup"><span data-stu-id="34410-165">Int32</span></span>|<span data-ttu-id="34410-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34410-166">Version of the device configuration.</span></span> <span data-ttu-id="34410-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34410-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34410-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="34410-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="34410-169">Int32</span><span class="sxs-lookup"><span data-stu-id="34410-169">Int32</span></span>|<span data-ttu-id="34410-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="34410-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="34410-171">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="34410-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="34410-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="34410-172">subjectNameFormat</span></span>|[<span data-ttu-id="34410-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="34410-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="34410-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="34410-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="34410-175">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="34410-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34410-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="34410-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="34410-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="34410-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="34410-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="34410-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="34410-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="34410-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="34410-180">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="34410-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34410-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="34410-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="34410-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="34410-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="34410-183">Int32</span><span class="sxs-lookup"><span data-stu-id="34410-183">Int32</span></span>|<span data-ttu-id="34410-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="34410-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="34410-185">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="34410-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="34410-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="34410-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="34410-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="34410-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="34410-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="34410-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="34410-189">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="34410-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34410-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="34410-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="34410-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="34410-191">scepServerUrls</span></span>|<span data-ttu-id="34410-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34410-192">String collection</span></span>|<span data-ttu-id="34410-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="34410-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="34410-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="34410-194">subjectNameFormatString</span></span>|<span data-ttu-id="34410-195">String</span><span class="sxs-lookup"><span data-stu-id="34410-195">String</span></span>|<span data-ttu-id="34410-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="34410-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="34410-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="34410-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="34410-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="34410-198">keyUsage</span></span>|[<span data-ttu-id="34410-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="34410-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="34410-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="34410-200">SCEP Key Usage.</span></span> <span data-ttu-id="34410-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="34410-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="34410-202">keySize</span><span class="sxs-lookup"><span data-stu-id="34410-202">keySize</span></span>|[<span data-ttu-id="34410-203">keySize</span><span class="sxs-lookup"><span data-stu-id="34410-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="34410-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="34410-204">SCEP Key Size.</span></span> <span data-ttu-id="34410-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="34410-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="34410-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="34410-206">hashAlgorithm</span></span>|[<span data-ttu-id="34410-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="34410-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="34410-208">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="34410-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="34410-209">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="34410-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="34410-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="34410-210">extendedKeyUsages</span></span>|<span data-ttu-id="34410-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="34410-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="34410-212">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="34410-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="34410-213">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="34410-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="34410-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="34410-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="34410-215">String</span><span class="sxs-lookup"><span data-stu-id="34410-215">String</span></span>|<span data-ttu-id="34410-216">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="34410-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="34410-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="34410-217">certificateStore</span></span>|[<span data-ttu-id="34410-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="34410-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="34410-219">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="34410-219">Target store certificate.</span></span> <span data-ttu-id="34410-220">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="34410-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="34410-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="34410-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="34410-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="34410-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="34410-223">Параметры альтернативного имени настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="34410-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="34410-224">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="34410-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="34410-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="34410-225">Response</span></span>
<span data-ttu-id="34410-226">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34410-226">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34410-227">Пример</span><span class="sxs-lookup"><span data-stu-id="34410-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="34410-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="34410-228">Request</span></span>
<span data-ttu-id="34410-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34410-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="34410-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="34410-230">Response</span></span>
<span data-ttu-id="34410-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34410-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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




