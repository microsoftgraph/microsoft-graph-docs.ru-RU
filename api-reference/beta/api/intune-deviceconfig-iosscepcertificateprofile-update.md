---
title: Обновление iosScepCertificateProfile
description: Обновление свойства объекта iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5f8ee6b856e2b8351059cd47de7bf8e9d2dddfd5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887201"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="fdcf0-103">Обновление iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fdcf0-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="fdcf0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdcf0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdcf0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdcf0-107">Обновление свойства объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fdcf0-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdcf0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdcf0-108">Prerequisites</span></span>
<span data-ttu-id="fdcf0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdcf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdcf0-111">Permission type</span></span>|<span data-ttu-id="fdcf0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdcf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdcf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdcf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdcf0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdcf0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdcf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdcf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdcf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-116">Not supported.</span></span>|
|<span data-ttu-id="fdcf0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdcf0-117">Application</span></span>|<span data-ttu-id="fdcf0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdcf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdcf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fdcf0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdcf0-120">Request headers</span></span>
|<span data-ttu-id="fdcf0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdcf0-121">Header</span></span>|<span data-ttu-id="fdcf0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdcf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdcf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdcf0-123">Authorization</span></span>|<span data-ttu-id="fdcf0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fdcf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdcf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdcf0-125">Accept</span></span>|<span data-ttu-id="fdcf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdcf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdcf0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdcf0-127">Request body</span></span>
<span data-ttu-id="fdcf0-128">В тексте запроса укажите представление JSON для объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fdcf0-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="fdcf0-129">В следующей таблице показаны свойства, которые необходимы для создания [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="fdcf0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdcf0-130">Property</span></span>|<span data-ttu-id="fdcf0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdcf0-131">Type</span></span>|<span data-ttu-id="fdcf0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdcf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdcf0-133">id</span><span class="sxs-lookup"><span data-stu-id="fdcf0-133">id</span></span>|<span data-ttu-id="fdcf0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fdcf0-134">String</span></span>|<span data-ttu-id="fdcf0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-135">Key of the entity.</span></span> <span data-ttu-id="fdcf0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdcf0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fdcf0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdcf0-138">DateTimeOffset</span></span>|<span data-ttu-id="fdcf0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fdcf0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fdcf0-141">roleScopeTagIds</span></span>|<span data-ttu-id="fdcf0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fdcf0-142">String collection</span></span>|<span data-ttu-id="fdcf0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fdcf0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fdcf0-145">supportsScopeTags</span></span>|<span data-ttu-id="fdcf0-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fdcf0-146">Boolean</span></span>|<span data-ttu-id="fdcf0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fdcf0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fdcf0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fdcf0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-150">This property is read-only.</span></span> <span data-ttu-id="fdcf0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdcf0-152">createdDateTime</span></span>|<span data-ttu-id="fdcf0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdcf0-153">DateTimeOffset</span></span>|<span data-ttu-id="fdcf0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-154">DateTime the object was created.</span></span> <span data-ttu-id="fdcf0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-156">описание</span><span class="sxs-lookup"><span data-stu-id="fdcf0-156">description</span></span>|<span data-ttu-id="fdcf0-157">Строка</span><span class="sxs-lookup"><span data-stu-id="fdcf0-157">String</span></span>|<span data-ttu-id="fdcf0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fdcf0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fdcf0-160">displayName</span></span>|<span data-ttu-id="fdcf0-161">Строка</span><span class="sxs-lookup"><span data-stu-id="fdcf0-161">String</span></span>|<span data-ttu-id="fdcf0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fdcf0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-164">version</span><span class="sxs-lookup"><span data-stu-id="fdcf0-164">version</span></span>|<span data-ttu-id="fdcf0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fdcf0-165">Int32</span></span>|<span data-ttu-id="fdcf0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-166">Version of the device configuration.</span></span> <span data-ttu-id="fdcf0-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdcf0-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fdcf0-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="fdcf0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="fdcf0-169">Int32</span></span>|<span data-ttu-id="fdcf0-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fdcf0-171">Допустимые значения от 1 до 99 унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fdcf0-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fdcf0-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fdcf0-172">subjectNameFormat</span></span>|[<span data-ttu-id="fdcf0-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fdcf0-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="fdcf0-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="fdcf0-175">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fdcf0-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="fdcf0-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fdcf0-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fdcf0-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fdcf0-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fdcf0-179">Тип имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="fdcf0-180">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fdcf0-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fdcf0-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fdcf0-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fdcf0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="fdcf0-183">Int32</span></span>|<span data-ttu-id="fdcf0-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fdcf0-185">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fdcf0-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fdcf0-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fdcf0-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fdcf0-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fdcf0-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fdcf0-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fdcf0-189">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fdcf0-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fdcf0-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="fdcf0-191">scepServerUrls</span></span>|<span data-ttu-id="fdcf0-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fdcf0-192">String collection</span></span>|<span data-ttu-id="fdcf0-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="fdcf0-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fdcf0-194">subjectNameFormatString</span></span>|<span data-ttu-id="fdcf0-195">Строка</span><span class="sxs-lookup"><span data-stu-id="fdcf0-195">String</span></span>|<span data-ttu-id="fdcf0-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="fdcf0-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="fdcf0-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="fdcf0-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="fdcf0-198">keyUsage</span></span>|[<span data-ttu-id="fdcf0-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="fdcf0-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="fdcf0-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-200">SCEP Key Usage.</span></span> <span data-ttu-id="fdcf0-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="fdcf0-202">keySize</span><span class="sxs-lookup"><span data-stu-id="fdcf0-202">keySize</span></span>|[<span data-ttu-id="fdcf0-203">keySize</span><span class="sxs-lookup"><span data-stu-id="fdcf0-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="fdcf0-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-204">SCEP Key Size.</span></span> <span data-ttu-id="fdcf0-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="fdcf0-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="fdcf0-206">extendedKeyUsages</span></span>|<span data-ttu-id="fdcf0-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fdcf0-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fdcf0-208">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="fdcf0-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fdcf0-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fdcf0-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fdcf0-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fdcf0-211">Строка</span><span class="sxs-lookup"><span data-stu-id="fdcf0-211">String</span></span>|<span data-ttu-id="fdcf0-212">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="fdcf0-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fdcf0-213">certificateStore</span></span>|[<span data-ttu-id="fdcf0-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fdcf0-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="fdcf0-215">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-215">Target store certificate.</span></span> <span data-ttu-id="fdcf0-216">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="fdcf0-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="fdcf0-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="fdcf0-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fdcf0-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="fdcf0-219">Параметры Alterantive имя настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="fdcf0-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fdcf0-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdcf0-221">Response</span></span>
<span data-ttu-id="fdcf0-222">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdcf0-223">Пример</span><span class="sxs-lookup"><span data-stu-id="fdcf0-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdcf0-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdcf0-224">Request</span></span>
<span data-ttu-id="fdcf0-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

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

### <a name="response"></a><span data-ttu-id="fdcf0-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdcf0-226">Response</span></span>
<span data-ttu-id="fdcf0-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fdcf0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





