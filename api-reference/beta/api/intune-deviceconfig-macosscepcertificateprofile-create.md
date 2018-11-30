---
title: Создание macOSScepCertificateProfile
description: Создание нового объекта macOSScepCertificateProfile.
ms.openlocfilehash: a0dfb409217ce38fca9b966c642c09ff89887f61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081895"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="7bd3c-103">Создание macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7bd3c-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="7bd3c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bd3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bd3c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bd3c-107">Создание нового объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7bd3c-107">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bd3c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7bd3c-108">Prerequisites</span></span>
<span data-ttu-id="7bd3c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bd3c-111">Permission type</span></span>|<span data-ttu-id="7bd3c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bd3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bd3c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bd3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bd3c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd3c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bd3c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bd3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bd3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-116">Not supported.</span></span>|
|<span data-ttu-id="7bd3c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bd3c-117">Application</span></span>|<span data-ttu-id="7bd3c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bd3c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bd3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7bd3c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bd3c-120">Request headers</span></span>
|<span data-ttu-id="7bd3c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bd3c-121">Header</span></span>|<span data-ttu-id="7bd3c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7bd3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bd3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd3c-123">Authorization</span></span>|<span data-ttu-id="7bd3c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7bd3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bd3c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7bd3c-125">Accept</span></span>|<span data-ttu-id="7bd3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bd3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bd3c-127">Request body</span></span>
<span data-ttu-id="7bd3c-128">В тексте запроса укажите представление JSON для объекта macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-128">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="7bd3c-129">В следующей таблице показаны свойства, которые необходимы для создания macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-129">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="7bd3c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bd3c-130">Property</span></span>|<span data-ttu-id="7bd3c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7bd3c-131">Type</span></span>|<span data-ttu-id="7bd3c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd3c-133">id</span><span class="sxs-lookup"><span data-stu-id="7bd3c-133">id</span></span>|<span data-ttu-id="7bd3c-134">String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-134">String</span></span>|<span data-ttu-id="7bd3c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-135">Key of the entity.</span></span> <span data-ttu-id="7bd3c-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd3c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7bd3c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd3c-138">DateTimeOffset</span></span>|<span data-ttu-id="7bd3c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7bd3c-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7bd3c-141">roleScopeTagIds</span></span>|<span data-ttu-id="7bd3c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-142">String collection</span></span>|<span data-ttu-id="7bd3c-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7bd3c-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7bd3c-145">supportsScopeTags</span></span>|<span data-ttu-id="7bd3c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7bd3c-146">Boolean</span></span>|<span data-ttu-id="7bd3c-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7bd3c-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7bd3c-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7bd3c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-150">This property is read-only.</span></span> <span data-ttu-id="7bd3c-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd3c-152">createdDateTime</span></span>|<span data-ttu-id="7bd3c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd3c-153">DateTimeOffset</span></span>|<span data-ttu-id="7bd3c-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-154">DateTime the object was created.</span></span> <span data-ttu-id="7bd3c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-156">описание</span><span class="sxs-lookup"><span data-stu-id="7bd3c-156">description</span></span>|<span data-ttu-id="7bd3c-157">String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-157">String</span></span>|<span data-ttu-id="7bd3c-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7bd3c-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7bd3c-160">displayName</span></span>|<span data-ttu-id="7bd3c-161">String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-161">String</span></span>|<span data-ttu-id="7bd3c-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7bd3c-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-164">version</span><span class="sxs-lookup"><span data-stu-id="7bd3c-164">version</span></span>|<span data-ttu-id="7bd3c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd3c-165">Int32</span></span>|<span data-ttu-id="7bd3c-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-166">Version of the device configuration.</span></span> <span data-ttu-id="7bd3c-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd3c-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="7bd3c-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="7bd3c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd3c-169">Int32</span></span>|<span data-ttu-id="7bd3c-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7bd3c-171">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7bd3c-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7bd3c-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7bd3c-172">subjectNameFormat</span></span>|[<span data-ttu-id="7bd3c-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7bd3c-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7bd3c-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="7bd3c-175">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd3c-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7bd3c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7bd3c-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7bd3c-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7bd3c-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7bd3c-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7bd3c-180">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd3c-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7bd3c-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7bd3c-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7bd3c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd3c-183">Int32</span></span>|<span data-ttu-id="7bd3c-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7bd3c-185">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7bd3c-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7bd3c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7bd3c-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7bd3c-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7bd3c-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7bd3c-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7bd3c-189">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd3c-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7bd3c-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="7bd3c-191">scepServerUrls</span></span>|<span data-ttu-id="7bd3c-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-192">String collection</span></span>|<span data-ttu-id="7bd3c-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="7bd3c-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7bd3c-194">subjectNameFormatString</span></span>|<span data-ttu-id="7bd3c-195">String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-195">String</span></span>|<span data-ttu-id="7bd3c-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7bd3c-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="7bd3c-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7bd3c-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="7bd3c-198">keyUsage</span></span>|[<span data-ttu-id="7bd3c-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="7bd3c-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7bd3c-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-200">SCEP Key Usage.</span></span> <span data-ttu-id="7bd3c-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7bd3c-202">keySize</span><span class="sxs-lookup"><span data-stu-id="7bd3c-202">keySize</span></span>|[<span data-ttu-id="7bd3c-203">keySize</span><span class="sxs-lookup"><span data-stu-id="7bd3c-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7bd3c-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-204">SCEP Key Size.</span></span> <span data-ttu-id="7bd3c-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7bd3c-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7bd3c-206">hashAlgorithm</span></span>|[<span data-ttu-id="7bd3c-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="7bd3c-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="7bd3c-208">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="7bd3c-209">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="7bd3c-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="7bd3c-210">extendedKeyUsages</span></span>|<span data-ttu-id="7bd3c-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7bd3c-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7bd3c-212">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="7bd3c-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7bd3c-213">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7bd3c-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7bd3c-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7bd3c-215">String</span><span class="sxs-lookup"><span data-stu-id="7bd3c-215">String</span></span>|<span data-ttu-id="7bd3c-216">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="7bd3c-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd3c-217">Response</span></span>
<span data-ttu-id="7bd3c-218">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-218">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bd3c-219">Пример</span><span class="sxs-lookup"><span data-stu-id="7bd3c-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bd3c-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bd3c-220">Request</span></span>
<span data-ttu-id="7bd3c-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bd3c-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="7bd3c-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd3c-222">Response</span></span>
<span data-ttu-id="7bd3c-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7bd3c-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





