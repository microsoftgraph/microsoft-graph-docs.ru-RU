---
title: Создание windowsPhone81SCEPCertificateProfile
description: Создание нового объекта windowsPhone81SCEPCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f18607a23c32ef6a42ed8037332d8308b7ac5751
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406978"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="f9662-103">Создание windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f9662-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="f9662-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9662-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9662-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9662-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9662-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9662-107">Создание нового объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9662-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9662-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f9662-108">Prerequisites</span></span>
<span data-ttu-id="f9662-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9662-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9662-111">Permission type</span></span>|<span data-ttu-id="f9662-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9662-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9662-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9662-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9662-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9662-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9662-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9662-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9662-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9662-116">Not supported.</span></span>|
|<span data-ttu-id="f9662-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9662-117">Application</span></span>|<span data-ttu-id="f9662-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9662-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9662-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9662-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f9662-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9662-120">Request headers</span></span>
|<span data-ttu-id="f9662-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9662-121">Header</span></span>|<span data-ttu-id="f9662-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9662-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9662-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9662-123">Authorization</span></span>|<span data-ttu-id="f9662-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f9662-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9662-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9662-125">Accept</span></span>|<span data-ttu-id="f9662-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9662-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9662-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9662-127">Request body</span></span>
<span data-ttu-id="f9662-128">В тексте запроса укажите представление JSON для объекта windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f9662-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="f9662-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f9662-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="f9662-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9662-130">Property</span></span>|<span data-ttu-id="f9662-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9662-131">Type</span></span>|<span data-ttu-id="f9662-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9662-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9662-133">id</span><span class="sxs-lookup"><span data-stu-id="f9662-133">id</span></span>|<span data-ttu-id="f9662-134">String</span><span class="sxs-lookup"><span data-stu-id="f9662-134">String</span></span>|<span data-ttu-id="f9662-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f9662-135">Key of the entity.</span></span> <span data-ttu-id="f9662-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9662-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f9662-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9662-138">DateTimeOffset</span></span>|<span data-ttu-id="f9662-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f9662-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f9662-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9662-141">roleScopeTagIds</span></span>|<span data-ttu-id="f9662-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f9662-142">String collection</span></span>|<span data-ttu-id="f9662-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f9662-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9662-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9662-145">supportsScopeTags</span></span>|<span data-ttu-id="f9662-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f9662-146">Boolean</span></span>|<span data-ttu-id="f9662-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f9662-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9662-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f9662-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9662-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f9662-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9662-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9662-150">This property is read-only.</span></span> <span data-ttu-id="f9662-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9662-152">createdDateTime</span></span>|<span data-ttu-id="f9662-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9662-153">DateTimeOffset</span></span>|<span data-ttu-id="f9662-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f9662-154">DateTime the object was created.</span></span> <span data-ttu-id="f9662-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-156">description</span><span class="sxs-lookup"><span data-stu-id="f9662-156">description</span></span>|<span data-ttu-id="f9662-157">String</span><span class="sxs-lookup"><span data-stu-id="f9662-157">String</span></span>|<span data-ttu-id="f9662-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f9662-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9662-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f9662-160">displayName</span></span>|<span data-ttu-id="f9662-161">String</span><span class="sxs-lookup"><span data-stu-id="f9662-161">String</span></span>|<span data-ttu-id="f9662-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f9662-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9662-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-164">version</span><span class="sxs-lookup"><span data-stu-id="f9662-164">version</span></span>|<span data-ttu-id="f9662-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f9662-165">Int32</span></span>|<span data-ttu-id="f9662-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f9662-166">Version of the device configuration.</span></span> <span data-ttu-id="f9662-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9662-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f9662-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f9662-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f9662-169">Int32</span></span>|<span data-ttu-id="f9662-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="f9662-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f9662-171">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9662-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9662-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f9662-172">keyStorageProvider</span></span>|[<span data-ttu-id="f9662-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f9662-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f9662-174">Поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="f9662-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="f9662-175">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f9662-176">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="f9662-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f9662-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f9662-177">subjectNameFormat</span></span>|[<span data-ttu-id="f9662-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f9662-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f9662-179">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f9662-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="f9662-180">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f9662-181">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f9662-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f9662-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f9662-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f9662-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f9662-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f9662-184">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f9662-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f9662-185">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f9662-186">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f9662-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f9662-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f9662-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f9662-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f9662-188">Int32</span></span>|<span data-ttu-id="f9662-189">Значение периода Validtiy сертификата.</span><span class="sxs-lookup"><span data-stu-id="f9662-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="f9662-190">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9662-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9662-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f9662-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f9662-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f9662-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f9662-193">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f9662-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f9662-194">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9662-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f9662-195">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f9662-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f9662-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f9662-196">extendedKeyUsages</span></span>|<span data-ttu-id="f9662-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f9662-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f9662-198">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="f9662-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f9662-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f9662-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f9662-200">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9662-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9662-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f9662-201">scepServerUrls</span></span>|<span data-ttu-id="f9662-202">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f9662-202">String collection</span></span>|<span data-ttu-id="f9662-203">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9662-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f9662-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f9662-204">subjectNameFormatString</span></span>|<span data-ttu-id="f9662-205">String</span><span class="sxs-lookup"><span data-stu-id="f9662-205">String</span></span>|<span data-ttu-id="f9662-206">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="f9662-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f9662-207">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="f9662-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f9662-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f9662-208">keyUsage</span></span>|[<span data-ttu-id="f9662-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f9662-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f9662-210">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="f9662-210">SCEP Key Usage.</span></span> <span data-ttu-id="f9662-211">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f9662-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f9662-212">keySize</span><span class="sxs-lookup"><span data-stu-id="f9662-212">keySize</span></span>|[<span data-ttu-id="f9662-213">keySize</span><span class="sxs-lookup"><span data-stu-id="f9662-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f9662-214">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9662-214">SCEP Key Size.</span></span> <span data-ttu-id="f9662-215">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f9662-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f9662-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f9662-216">hashAlgorithm</span></span>|[<span data-ttu-id="f9662-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="f9662-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f9662-218">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9662-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f9662-219">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f9662-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f9662-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f9662-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f9662-221">String</span><span class="sxs-lookup"><span data-stu-id="f9662-221">String</span></span>|<span data-ttu-id="f9662-222">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="f9662-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f9662-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9662-223">Response</span></span>
<span data-ttu-id="f9662-224">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9662-224">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9662-225">Пример</span><span class="sxs-lookup"><span data-stu-id="f9662-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9662-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9662-226">Request</span></span>
<span data-ttu-id="f9662-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9662-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="f9662-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9662-228">Response</span></span>
<span data-ttu-id="f9662-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f9662-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




