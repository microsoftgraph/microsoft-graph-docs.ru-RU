---
title: Создание iosScepCertificateProfile
description: Создание нового объекта iosScepCertificateProfile.
ms.openlocfilehash: 64f0db48d1c1a96883942513d4b822850d2269e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076204"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="0a722-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0a722-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="0a722-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a722-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a722-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a722-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a722-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a722-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a722-107">Создание нового объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0a722-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a722-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a722-108">Prerequisites</span></span>
<span data-ttu-id="0a722-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a722-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a722-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a722-111">Permission type</span></span>|<span data-ttu-id="0a722-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a722-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a722-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a722-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a722-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a722-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a722-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a722-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a722-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a722-116">Not supported.</span></span>|
|<span data-ttu-id="0a722-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a722-117">Application</span></span>|<span data-ttu-id="0a722-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a722-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a722-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a722-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a722-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a722-120">Request headers</span></span>
|<span data-ttu-id="0a722-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a722-121">Header</span></span>|<span data-ttu-id="0a722-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a722-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a722-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a722-123">Authorization</span></span>|<span data-ttu-id="0a722-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0a722-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a722-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a722-125">Accept</span></span>|<span data-ttu-id="0a722-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a722-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a722-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a722-127">Request body</span></span>
<span data-ttu-id="0a722-128">В тексте запроса укажите представление JSON для объекта iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0a722-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="0a722-129">В следующей таблице показаны свойства, которые необходимы для создания iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="0a722-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="0a722-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a722-130">Property</span></span>|<span data-ttu-id="0a722-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a722-131">Type</span></span>|<span data-ttu-id="0a722-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a722-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a722-133">id</span><span class="sxs-lookup"><span data-stu-id="0a722-133">id</span></span>|<span data-ttu-id="0a722-134">String</span><span class="sxs-lookup"><span data-stu-id="0a722-134">String</span></span>|<span data-ttu-id="0a722-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a722-135">Key of the entity.</span></span> <span data-ttu-id="0a722-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a722-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0a722-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a722-138">DateTimeOffset</span></span>|<span data-ttu-id="0a722-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0a722-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0a722-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a722-141">roleScopeTagIds</span></span>|<span data-ttu-id="0a722-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a722-142">String collection</span></span>|<span data-ttu-id="0a722-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0a722-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a722-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a722-145">supportsScopeTags</span></span>|<span data-ttu-id="0a722-146">Логический</span><span class="sxs-lookup"><span data-stu-id="0a722-146">Boolean</span></span>|<span data-ttu-id="0a722-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="0a722-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a722-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="0a722-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a722-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0a722-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a722-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a722-150">This property is read-only.</span></span> <span data-ttu-id="0a722-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a722-152">createdDateTime</span></span>|<span data-ttu-id="0a722-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a722-153">DateTimeOffset</span></span>|<span data-ttu-id="0a722-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0a722-154">DateTime the object was created.</span></span> <span data-ttu-id="0a722-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-156">описание</span><span class="sxs-lookup"><span data-stu-id="0a722-156">description</span></span>|<span data-ttu-id="0a722-157">String</span><span class="sxs-lookup"><span data-stu-id="0a722-157">String</span></span>|<span data-ttu-id="0a722-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0a722-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a722-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0a722-160">displayName</span></span>|<span data-ttu-id="0a722-161">String</span><span class="sxs-lookup"><span data-stu-id="0a722-161">String</span></span>|<span data-ttu-id="0a722-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0a722-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a722-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-164">version</span><span class="sxs-lookup"><span data-stu-id="0a722-164">version</span></span>|<span data-ttu-id="0a722-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0a722-165">Int32</span></span>|<span data-ttu-id="0a722-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0a722-166">Version of the device configuration.</span></span> <span data-ttu-id="0a722-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a722-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0a722-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="0a722-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0a722-169">Int32</span></span>|<span data-ttu-id="0a722-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="0a722-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0a722-171">Допустимые значения от 1 до 99 унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a722-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0a722-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0a722-172">subjectNameFormat</span></span>|[<span data-ttu-id="0a722-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0a722-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="0a722-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0a722-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="0a722-175">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="0a722-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="0a722-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="0a722-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0a722-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0a722-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0a722-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0a722-179">Тип имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0a722-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="0a722-180">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="0a722-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0a722-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0a722-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0a722-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0a722-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0a722-183">Int32</span></span>|<span data-ttu-id="0a722-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0a722-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0a722-185">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0a722-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0a722-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0a722-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0a722-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0a722-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0a722-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0a722-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0a722-189">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0a722-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="0a722-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0a722-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0a722-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="0a722-191">scepServerUrls</span></span>|<span data-ttu-id="0a722-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a722-192">String collection</span></span>|<span data-ttu-id="0a722-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a722-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="0a722-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0a722-194">subjectNameFormatString</span></span>|<span data-ttu-id="0a722-195">String</span><span class="sxs-lookup"><span data-stu-id="0a722-195">String</span></span>|<span data-ttu-id="0a722-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="0a722-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="0a722-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="0a722-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="0a722-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="0a722-198">keyUsage</span></span>|[<span data-ttu-id="0a722-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="0a722-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="0a722-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="0a722-200">SCEP Key Usage.</span></span> <span data-ttu-id="0a722-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="0a722-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="0a722-202">keySize</span><span class="sxs-lookup"><span data-stu-id="0a722-202">keySize</span></span>|[<span data-ttu-id="0a722-203">keySize</span><span class="sxs-lookup"><span data-stu-id="0a722-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="0a722-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="0a722-204">SCEP Key Size.</span></span> <span data-ttu-id="0a722-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="0a722-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="0a722-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0a722-206">extendedKeyUsages</span></span>|<span data-ttu-id="0a722-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a722-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0a722-208">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="0a722-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0a722-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0a722-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0a722-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0a722-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0a722-211">String</span><span class="sxs-lookup"><span data-stu-id="0a722-211">String</span></span>|<span data-ttu-id="0a722-212">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="0a722-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="0a722-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0a722-213">certificateStore</span></span>|[<span data-ttu-id="0a722-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0a722-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="0a722-215">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="0a722-215">Target store certificate.</span></span> <span data-ttu-id="0a722-216">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0a722-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0a722-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="0a722-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="0a722-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a722-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0a722-219">Параметры Alterantive имя настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="0a722-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="0a722-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0a722-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0a722-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a722-221">Response</span></span>
<span data-ttu-id="0a722-222">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a722-222">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a722-223">Пример</span><span class="sxs-lookup"><span data-stu-id="0a722-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a722-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a722-224">Request</span></span>
<span data-ttu-id="0a722-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a722-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="0a722-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a722-226">Response</span></span>
<span data-ttu-id="0a722-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0a722-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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





