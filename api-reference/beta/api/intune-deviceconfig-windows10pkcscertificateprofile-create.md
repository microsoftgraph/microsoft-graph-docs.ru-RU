---
title: Создание windows10PkcsCertificateProfile
description: Создание нового объекта windows10PkcsCertificateProfile.
author: tfitzmac
ms.openlocfilehash: 4ca3199e8c0865ed3a68320b2d46ee9f0bf084f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338187"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="3c2eb-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3c2eb-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="3c2eb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c2eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c2eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c2eb-107">Создание нового объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3c2eb-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c2eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c2eb-108">Prerequisites</span></span>
<span data-ttu-id="3c2eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c2eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c2eb-111">Permission type</span></span>|<span data-ttu-id="3c2eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c2eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c2eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c2eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c2eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c2eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c2eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c2eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-116">Not supported.</span></span>|
|<span data-ttu-id="3c2eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c2eb-117">Application</span></span>|<span data-ttu-id="3c2eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c2eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c2eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c2eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c2eb-120">Request headers</span></span>
|<span data-ttu-id="3c2eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c2eb-121">Header</span></span>|<span data-ttu-id="3c2eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c2eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c2eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c2eb-123">Authorization</span></span>|<span data-ttu-id="3c2eb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c2eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c2eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c2eb-125">Accept</span></span>|<span data-ttu-id="3c2eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c2eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c2eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c2eb-127">Request body</span></span>
<span data-ttu-id="3c2eb-128">В тексте запроса укажите представление JSON для объекта windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="3c2eb-129">В следующей таблице показаны свойства, которые необходимы для создания windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="3c2eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c2eb-130">Property</span></span>|<span data-ttu-id="3c2eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c2eb-131">Type</span></span>|<span data-ttu-id="3c2eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c2eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2eb-133">id</span><span class="sxs-lookup"><span data-stu-id="3c2eb-133">id</span></span>|<span data-ttu-id="3c2eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2eb-134">String</span></span>|<span data-ttu-id="3c2eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-135">Key of the entity.</span></span> <span data-ttu-id="3c2eb-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2eb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3c2eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2eb-138">DateTimeOffset</span></span>|<span data-ttu-id="3c2eb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3c2eb-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c2eb-141">roleScopeTagIds</span></span>|<span data-ttu-id="3c2eb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c2eb-142">String collection</span></span>|<span data-ttu-id="3c2eb-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3c2eb-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3c2eb-145">supportsScopeTags</span></span>|<span data-ttu-id="3c2eb-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-146">Boolean</span></span>|<span data-ttu-id="3c2eb-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3c2eb-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3c2eb-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3c2eb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-150">This property is read-only.</span></span> <span data-ttu-id="3c2eb-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2eb-152">createdDateTime</span></span>|<span data-ttu-id="3c2eb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2eb-153">DateTimeOffset</span></span>|<span data-ttu-id="3c2eb-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-154">DateTime the object was created.</span></span> <span data-ttu-id="3c2eb-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-156">описание</span><span class="sxs-lookup"><span data-stu-id="3c2eb-156">description</span></span>|<span data-ttu-id="3c2eb-157">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2eb-157">String</span></span>|<span data-ttu-id="3c2eb-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c2eb-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3c2eb-160">displayName</span></span>|<span data-ttu-id="3c2eb-161">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2eb-161">String</span></span>|<span data-ttu-id="3c2eb-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c2eb-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-164">version</span><span class="sxs-lookup"><span data-stu-id="3c2eb-164">version</span></span>|<span data-ttu-id="3c2eb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3c2eb-165">Int32</span></span>|<span data-ttu-id="3c2eb-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-166">Version of the device configuration.</span></span> <span data-ttu-id="3c2eb-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2eb-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3c2eb-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3c2eb-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3c2eb-169">Int32</span></span>|<span data-ttu-id="3c2eb-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3c2eb-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3c2eb-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3c2eb-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="3c2eb-172">keyStorageProvider</span></span>|[<span data-ttu-id="3c2eb-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3c2eb-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="3c2eb-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3c2eb-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="3c2eb-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3c2eb-176">subjectNameFormat</span></span>|[<span data-ttu-id="3c2eb-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3c2eb-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3c2eb-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3c2eb-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3c2eb-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3c2eb-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3c2eb-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3c2eb-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3c2eb-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3c2eb-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3c2eb-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3c2eb-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3c2eb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3c2eb-185">Int32</span></span>|<span data-ttu-id="3c2eb-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3c2eb-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3c2eb-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3c2eb-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3c2eb-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3c2eb-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3c2eb-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3c2eb-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3c2eb-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="3c2eb-191">certificationAuthority</span></span>|<span data-ttu-id="3c2eb-192">String.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-192">String</span></span>|<span data-ttu-id="3c2eb-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3c2eb-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="3c2eb-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="3c2eb-194">certificationAuthorityName</span></span>|<span data-ttu-id="3c2eb-195">String.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-195">String</span></span>|<span data-ttu-id="3c2eb-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3c2eb-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="3c2eb-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="3c2eb-197">certificateTemplateName</span></span>|<span data-ttu-id="3c2eb-198">String.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-198">String</span></span>|<span data-ttu-id="3c2eb-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="3c2eb-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="3c2eb-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3c2eb-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3c2eb-201">String.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-201">String</span></span>|<span data-ttu-id="3c2eb-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="3c2eb-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3c2eb-203">extendedKeyUsages</span></span>|<span data-ttu-id="3c2eb-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3c2eb-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3c2eb-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="3c2eb-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3c2eb-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3c2eb-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c2eb-207">Response</span></span>
<span data-ttu-id="3c2eb-208">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-208">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c2eb-209">Пример</span><span class="sxs-lookup"><span data-stu-id="3c2eb-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c2eb-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c2eb-210">Request</span></span>
<span data-ttu-id="3c2eb-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3c2eb-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c2eb-212">Response</span></span>
<span data-ttu-id="3c2eb-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c2eb-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```





