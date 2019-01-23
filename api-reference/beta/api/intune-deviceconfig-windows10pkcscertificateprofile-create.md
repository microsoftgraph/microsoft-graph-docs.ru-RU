---
title: Создание windows10PkcsCertificateProfile
description: Создание нового объекта windows10PkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: baa12b444c52dd78b8d92944b9296a1a25e38f6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416435"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="a058c-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a058c-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="a058c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a058c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a058c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a058c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a058c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a058c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a058c-107">Создание нового объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a058c-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a058c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a058c-108">Prerequisites</span></span>
<span data-ttu-id="a058c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a058c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a058c-111">Permission type</span></span>|<span data-ttu-id="a058c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a058c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a058c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a058c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a058c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a058c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a058c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a058c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a058c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a058c-116">Not supported.</span></span>|
|<span data-ttu-id="a058c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a058c-117">Application</span></span>|<span data-ttu-id="a058c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a058c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a058c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a058c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a058c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a058c-120">Request headers</span></span>
|<span data-ttu-id="a058c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a058c-121">Header</span></span>|<span data-ttu-id="a058c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a058c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a058c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a058c-123">Authorization</span></span>|<span data-ttu-id="a058c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a058c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a058c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a058c-125">Accept</span></span>|<span data-ttu-id="a058c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a058c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a058c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a058c-127">Request body</span></span>
<span data-ttu-id="a058c-128">В тексте запроса укажите представление JSON для объекта windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a058c-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="a058c-129">В следующей таблице показаны свойства, которые необходимы для создания windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a058c-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="a058c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a058c-130">Property</span></span>|<span data-ttu-id="a058c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a058c-131">Type</span></span>|<span data-ttu-id="a058c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a058c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a058c-133">id</span><span class="sxs-lookup"><span data-stu-id="a058c-133">id</span></span>|<span data-ttu-id="a058c-134">String</span><span class="sxs-lookup"><span data-stu-id="a058c-134">String</span></span>|<span data-ttu-id="a058c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a058c-135">Key of the entity.</span></span> <span data-ttu-id="a058c-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a058c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a058c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a058c-138">DateTimeOffset</span></span>|<span data-ttu-id="a058c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a058c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a058c-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a058c-141">roleScopeTagIds</span></span>|<span data-ttu-id="a058c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a058c-142">String collection</span></span>|<span data-ttu-id="a058c-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a058c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a058c-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a058c-145">supportsScopeTags</span></span>|<span data-ttu-id="a058c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a058c-146">Boolean</span></span>|<span data-ttu-id="a058c-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a058c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a058c-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a058c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a058c-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a058c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a058c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a058c-150">This property is read-only.</span></span> <span data-ttu-id="a058c-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a058c-152">createdDateTime</span></span>|<span data-ttu-id="a058c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a058c-153">DateTimeOffset</span></span>|<span data-ttu-id="a058c-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a058c-154">DateTime the object was created.</span></span> <span data-ttu-id="a058c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-156">description</span><span class="sxs-lookup"><span data-stu-id="a058c-156">description</span></span>|<span data-ttu-id="a058c-157">String</span><span class="sxs-lookup"><span data-stu-id="a058c-157">String</span></span>|<span data-ttu-id="a058c-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a058c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a058c-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a058c-160">displayName</span></span>|<span data-ttu-id="a058c-161">String</span><span class="sxs-lookup"><span data-stu-id="a058c-161">String</span></span>|<span data-ttu-id="a058c-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a058c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a058c-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-164">version</span><span class="sxs-lookup"><span data-stu-id="a058c-164">version</span></span>|<span data-ttu-id="a058c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a058c-165">Int32</span></span>|<span data-ttu-id="a058c-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a058c-166">Version of the device configuration.</span></span> <span data-ttu-id="a058c-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a058c-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a058c-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a058c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a058c-169">Int32</span></span>|<span data-ttu-id="a058c-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="a058c-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a058c-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a058c-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a058c-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a058c-172">keyStorageProvider</span></span>|[<span data-ttu-id="a058c-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a058c-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a058c-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a058c-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a058c-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a058c-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a058c-176">subjectNameFormat</span></span>|[<span data-ttu-id="a058c-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a058c-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a058c-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a058c-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a058c-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a058c-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a058c-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a058c-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a058c-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a058c-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a058c-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a058c-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a058c-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a058c-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a058c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a058c-185">Int32</span></span>|<span data-ttu-id="a058c-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a058c-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a058c-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a058c-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a058c-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a058c-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a058c-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a058c-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a058c-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a058c-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a058c-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="a058c-191">certificationAuthority</span></span>|<span data-ttu-id="a058c-192">String</span><span class="sxs-lookup"><span data-stu-id="a058c-192">String</span></span>|<span data-ttu-id="a058c-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="a058c-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="a058c-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="a058c-194">certificationAuthorityName</span></span>|<span data-ttu-id="a058c-195">String</span><span class="sxs-lookup"><span data-stu-id="a058c-195">String</span></span>|<span data-ttu-id="a058c-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="a058c-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="a058c-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="a058c-197">certificateTemplateName</span></span>|<span data-ttu-id="a058c-198">String</span><span class="sxs-lookup"><span data-stu-id="a058c-198">String</span></span>|<span data-ttu-id="a058c-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="a058c-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="a058c-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a058c-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a058c-201">String</span><span class="sxs-lookup"><span data-stu-id="a058c-201">String</span></span>|<span data-ttu-id="a058c-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="a058c-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="a058c-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a058c-203">extendedKeyUsages</span></span>|<span data-ttu-id="a058c-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a058c-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a058c-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="a058c-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a058c-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a058c-206">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a058c-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="a058c-207">Response</span></span>
<span data-ttu-id="a058c-208">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a058c-208">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a058c-209">Пример</span><span class="sxs-lookup"><span data-stu-id="a058c-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="a058c-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="a058c-210">Request</span></span>
<span data-ttu-id="a058c-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a058c-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="a058c-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="a058c-212">Response</span></span>
<span data-ttu-id="a058c-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a058c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




