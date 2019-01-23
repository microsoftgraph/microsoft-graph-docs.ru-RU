---
title: Обновление windows81SCEPCertificateProfile
description: Обновление свойства объекта windows81SCEPCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9e1efc6ca53b28cd2d1e0b8254a439959866ee94
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396611"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="ffcfa-103">Обновление windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ffcfa-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="ffcfa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ffcfa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffcfa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffcfa-107">Обновление свойства объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ffcfa-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffcfa-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ffcfa-108">Prerequisites</span></span>
<span data-ttu-id="ffcfa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ffcfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffcfa-111">Permission type</span></span>|<span data-ttu-id="ffcfa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffcfa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffcfa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffcfa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffcfa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffcfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-116">Not supported.</span></span>|
|<span data-ttu-id="ffcfa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffcfa-117">Application</span></span>|<span data-ttu-id="ffcfa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffcfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffcfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ffcfa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffcfa-120">Request headers</span></span>
|<span data-ttu-id="ffcfa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffcfa-121">Header</span></span>|<span data-ttu-id="ffcfa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffcfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffcfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffcfa-123">Authorization</span></span>|<span data-ttu-id="ffcfa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffcfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffcfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffcfa-125">Accept</span></span>|<span data-ttu-id="ffcfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffcfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffcfa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffcfa-127">Request body</span></span>
<span data-ttu-id="ffcfa-128">В тексте запроса укажите представление JSON для объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ffcfa-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="ffcfa-129">В следующей таблице показаны свойства, которые необходимы для создания [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="ffcfa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffcfa-130">Property</span></span>|<span data-ttu-id="ffcfa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ffcfa-131">Type</span></span>|<span data-ttu-id="ffcfa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffcfa-133">id</span><span class="sxs-lookup"><span data-stu-id="ffcfa-133">id</span></span>|<span data-ttu-id="ffcfa-134">String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-134">String</span></span>|<span data-ttu-id="ffcfa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-135">Key of the entity.</span></span> <span data-ttu-id="ffcfa-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffcfa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ffcfa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffcfa-138">DateTimeOffset</span></span>|<span data-ttu-id="ffcfa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ffcfa-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ffcfa-141">roleScopeTagIds</span></span>|<span data-ttu-id="ffcfa-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-142">String collection</span></span>|<span data-ttu-id="ffcfa-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ffcfa-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ffcfa-145">supportsScopeTags</span></span>|<span data-ttu-id="ffcfa-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ffcfa-146">Boolean</span></span>|<span data-ttu-id="ffcfa-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ffcfa-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ffcfa-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ffcfa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-150">This property is read-only.</span></span> <span data-ttu-id="ffcfa-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffcfa-152">createdDateTime</span></span>|<span data-ttu-id="ffcfa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffcfa-153">DateTimeOffset</span></span>|<span data-ttu-id="ffcfa-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-154">DateTime the object was created.</span></span> <span data-ttu-id="ffcfa-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-156">description</span><span class="sxs-lookup"><span data-stu-id="ffcfa-156">description</span></span>|<span data-ttu-id="ffcfa-157">String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-157">String</span></span>|<span data-ttu-id="ffcfa-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ffcfa-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ffcfa-160">displayName</span></span>|<span data-ttu-id="ffcfa-161">String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-161">String</span></span>|<span data-ttu-id="ffcfa-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ffcfa-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-164">version</span><span class="sxs-lookup"><span data-stu-id="ffcfa-164">version</span></span>|<span data-ttu-id="ffcfa-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ffcfa-165">Int32</span></span>|<span data-ttu-id="ffcfa-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-166">Version of the device configuration.</span></span> <span data-ttu-id="ffcfa-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffcfa-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ffcfa-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="ffcfa-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ffcfa-169">Int32</span></span>|<span data-ttu-id="ffcfa-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ffcfa-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ffcfa-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ffcfa-172">keyStorageProvider</span></span>|[<span data-ttu-id="ffcfa-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ffcfa-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ffcfa-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ffcfa-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ffcfa-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ffcfa-176">subjectNameFormat</span></span>|[<span data-ttu-id="ffcfa-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ffcfa-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ffcfa-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ffcfa-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ffcfa-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ffcfa-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ffcfa-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ffcfa-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ffcfa-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ffcfa-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ffcfa-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ffcfa-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ffcfa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ffcfa-185">Int32</span></span>|<span data-ttu-id="ffcfa-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ffcfa-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ffcfa-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ffcfa-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ffcfa-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ffcfa-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ffcfa-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ffcfa-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ffcfa-191">extendedKeyUsages</span></span>|<span data-ttu-id="ffcfa-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ffcfa-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ffcfa-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="ffcfa-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ffcfa-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ffcfa-195">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ffcfa-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ffcfa-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ffcfa-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ffcfa-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ffcfa-198">Параметры Alterantive имя настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="ffcfa-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ffcfa-200">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ffcfa-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ffcfa-201">scepServerUrls</span></span>|<span data-ttu-id="ffcfa-202">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-202">String collection</span></span>|<span data-ttu-id="ffcfa-203">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ffcfa-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ffcfa-204">subjectNameFormatString</span></span>|<span data-ttu-id="ffcfa-205">String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-205">String</span></span>|<span data-ttu-id="ffcfa-206">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ffcfa-207">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="ffcfa-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ffcfa-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="ffcfa-208">keyUsage</span></span>|[<span data-ttu-id="ffcfa-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ffcfa-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ffcfa-210">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-210">SCEP Key Usage.</span></span> <span data-ttu-id="ffcfa-211">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ffcfa-212">keySize</span><span class="sxs-lookup"><span data-stu-id="ffcfa-212">keySize</span></span>|[<span data-ttu-id="ffcfa-213">keySize</span><span class="sxs-lookup"><span data-stu-id="ffcfa-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ffcfa-214">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-214">SCEP Key Size.</span></span> <span data-ttu-id="ffcfa-215">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ffcfa-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ffcfa-216">hashAlgorithm</span></span>|[<span data-ttu-id="ffcfa-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ffcfa-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ffcfa-218">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ffcfa-219">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ffcfa-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ffcfa-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ffcfa-221">String</span><span class="sxs-lookup"><span data-stu-id="ffcfa-221">String</span></span>|<span data-ttu-id="ffcfa-222">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ffcfa-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ffcfa-223">certificateStore</span></span>|[<span data-ttu-id="ffcfa-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ffcfa-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ffcfa-225">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-225">Target store certificate.</span></span> <span data-ttu-id="ffcfa-226">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="ffcfa-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffcfa-227">Response</span></span>
<span data-ttu-id="ffcfa-228">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-228">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffcfa-229">Пример</span><span class="sxs-lookup"><span data-stu-id="ffcfa-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffcfa-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffcfa-230">Request</span></span>
<span data-ttu-id="ffcfa-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1251

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="ffcfa-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffcfa-232">Response</span></span>
<span data-ttu-id="ffcfa-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```




