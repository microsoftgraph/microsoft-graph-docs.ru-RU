---
title: Обновление macOSScepCertificateProfile
description: Обновление свойства объекта macOSScepCertificateProfile.
ms.openlocfilehash: 459e3eaa90533320b5d6039802d9dca81958ef04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082065"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="cb1e2-103">Обновление macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="cb1e2-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="cb1e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb1e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb1e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb1e2-107">Обновление свойства объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cb1e2-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb1e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb1e2-108">Prerequisites</span></span>
<span data-ttu-id="cb1e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb1e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb1e2-111">Permission type</span></span>|<span data-ttu-id="cb1e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb1e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb1e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb1e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb1e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb1e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb1e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb1e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb1e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-116">Not supported.</span></span>|
|<span data-ttu-id="cb1e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb1e2-117">Application</span></span>|<span data-ttu-id="cb1e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb1e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb1e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb1e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb1e2-120">Request headers</span></span>
|<span data-ttu-id="cb1e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb1e2-121">Header</span></span>|<span data-ttu-id="cb1e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb1e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb1e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb1e2-123">Authorization</span></span>|<span data-ttu-id="cb1e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb1e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb1e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb1e2-125">Accept</span></span>|<span data-ttu-id="cb1e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb1e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb1e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb1e2-127">Request body</span></span>
<span data-ttu-id="cb1e2-128">В тексте запроса укажите представление JSON для объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cb1e2-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="cb1e2-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="cb1e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb1e2-130">Property</span></span>|<span data-ttu-id="cb1e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb1e2-131">Type</span></span>|<span data-ttu-id="cb1e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb1e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb1e2-133">id</span><span class="sxs-lookup"><span data-stu-id="cb1e2-133">id</span></span>|<span data-ttu-id="cb1e2-134">String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-134">String</span></span>|<span data-ttu-id="cb1e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-135">Key of the entity.</span></span> <span data-ttu-id="cb1e2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb1e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cb1e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb1e2-138">DateTimeOffset</span></span>|<span data-ttu-id="cb1e2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cb1e2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb1e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="cb1e2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-142">String collection</span></span>|<span data-ttu-id="cb1e2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb1e2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cb1e2-145">supportsScopeTags</span></span>|<span data-ttu-id="cb1e2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="cb1e2-146">Boolean</span></span>|<span data-ttu-id="cb1e2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb1e2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb1e2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb1e2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-150">This property is read-only.</span></span> <span data-ttu-id="cb1e2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb1e2-152">createdDateTime</span></span>|<span data-ttu-id="cb1e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb1e2-153">DateTimeOffset</span></span>|<span data-ttu-id="cb1e2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-154">DateTime the object was created.</span></span> <span data-ttu-id="cb1e2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-156">описание</span><span class="sxs-lookup"><span data-stu-id="cb1e2-156">description</span></span>|<span data-ttu-id="cb1e2-157">String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-157">String</span></span>|<span data-ttu-id="cb1e2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb1e2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cb1e2-160">displayName</span></span>|<span data-ttu-id="cb1e2-161">String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-161">String</span></span>|<span data-ttu-id="cb1e2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb1e2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-164">version</span><span class="sxs-lookup"><span data-stu-id="cb1e2-164">version</span></span>|<span data-ttu-id="cb1e2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cb1e2-165">Int32</span></span>|<span data-ttu-id="cb1e2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-166">Version of the device configuration.</span></span> <span data-ttu-id="cb1e2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb1e2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="cb1e2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="cb1e2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="cb1e2-169">Int32</span></span>|<span data-ttu-id="cb1e2-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="cb1e2-171">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cb1e2-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cb1e2-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cb1e2-172">subjectNameFormat</span></span>|[<span data-ttu-id="cb1e2-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cb1e2-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="cb1e2-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="cb1e2-175">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="cb1e2-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="cb1e2-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cb1e2-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="cb1e2-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cb1e2-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cb1e2-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="cb1e2-180">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="cb1e2-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="cb1e2-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="cb1e2-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="cb1e2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cb1e2-183">Int32</span></span>|<span data-ttu-id="cb1e2-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="cb1e2-185">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cb1e2-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cb1e2-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cb1e2-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="cb1e2-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cb1e2-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cb1e2-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="cb1e2-189">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="cb1e2-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="cb1e2-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="cb1e2-191">scepServerUrls</span></span>|<span data-ttu-id="cb1e2-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-192">String collection</span></span>|<span data-ttu-id="cb1e2-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="cb1e2-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cb1e2-194">subjectNameFormatString</span></span>|<span data-ttu-id="cb1e2-195">String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-195">String</span></span>|<span data-ttu-id="cb1e2-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="cb1e2-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="cb1e2-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="cb1e2-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="cb1e2-198">keyUsage</span></span>|[<span data-ttu-id="cb1e2-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="cb1e2-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="cb1e2-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-200">SCEP Key Usage.</span></span> <span data-ttu-id="cb1e2-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="cb1e2-202">keySize</span><span class="sxs-lookup"><span data-stu-id="cb1e2-202">keySize</span></span>|[<span data-ttu-id="cb1e2-203">keySize</span><span class="sxs-lookup"><span data-stu-id="cb1e2-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="cb1e2-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-204">SCEP Key Size.</span></span> <span data-ttu-id="cb1e2-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="cb1e2-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="cb1e2-206">hashAlgorithm</span></span>|[<span data-ttu-id="cb1e2-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="cb1e2-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="cb1e2-208">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="cb1e2-209">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="cb1e2-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="cb1e2-210">extendedKeyUsages</span></span>|<span data-ttu-id="cb1e2-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cb1e2-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="cb1e2-212">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="cb1e2-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="cb1e2-213">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cb1e2-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cb1e2-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="cb1e2-215">String</span><span class="sxs-lookup"><span data-stu-id="cb1e2-215">String</span></span>|<span data-ttu-id="cb1e2-216">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="cb1e2-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb1e2-217">Response</span></span>
<span data-ttu-id="cb1e2-218">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-218">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb1e2-219">Пример</span><span class="sxs-lookup"><span data-stu-id="cb1e2-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb1e2-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb1e2-220">Request</span></span>
<span data-ttu-id="cb1e2-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb1e2-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 963

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="cb1e2-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb1e2-222">Response</span></span>
<span data-ttu-id="cb1e2-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb1e2-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





