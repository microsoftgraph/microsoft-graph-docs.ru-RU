---
title: Обновление androidWorkProfilePkcsCertificateProfile
description: Обновление свойства объекта androidWorkProfilePkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6869e772bed3a2369e7a24948f140ae4904c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414503"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="b3261-103">Обновление androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b3261-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="b3261-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3261-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3261-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3261-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3261-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3261-107">Обновление свойства объекта [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b3261-107">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3261-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="b3261-108">Prerequisites</span></span>
<span data-ttu-id="b3261-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3261-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3261-111">Permission type</span></span>|<span data-ttu-id="b3261-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3261-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3261-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3261-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3261-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3261-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3261-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3261-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3261-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3261-116">Not supported.</span></span>|
|<span data-ttu-id="b3261-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3261-117">Application</span></span>|<span data-ttu-id="b3261-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3261-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3261-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3261-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3261-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3261-120">Request headers</span></span>
|<span data-ttu-id="b3261-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3261-121">Header</span></span>|<span data-ttu-id="b3261-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3261-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3261-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3261-123">Authorization</span></span>|<span data-ttu-id="b3261-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b3261-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3261-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3261-125">Accept</span></span>|<span data-ttu-id="b3261-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3261-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3261-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3261-127">Request body</span></span>
<span data-ttu-id="b3261-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b3261-128">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b3261-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-129">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b3261-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3261-130">Property</span></span>|<span data-ttu-id="b3261-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3261-131">Type</span></span>|<span data-ttu-id="b3261-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3261-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3261-133">id</span><span class="sxs-lookup"><span data-stu-id="b3261-133">id</span></span>|<span data-ttu-id="b3261-134">String</span><span class="sxs-lookup"><span data-stu-id="b3261-134">String</span></span>|<span data-ttu-id="b3261-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3261-135">Key of the entity.</span></span> <span data-ttu-id="b3261-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3261-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3261-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3261-138">DateTimeOffset</span></span>|<span data-ttu-id="b3261-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b3261-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3261-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3261-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3261-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3261-142">String collection</span></span>|<span data-ttu-id="b3261-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b3261-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3261-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3261-145">supportsScopeTags</span></span>|<span data-ttu-id="b3261-146">Логический</span><span class="sxs-lookup"><span data-stu-id="b3261-146">Boolean</span></span>|<span data-ttu-id="b3261-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="b3261-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3261-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="b3261-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3261-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b3261-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3261-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3261-150">This property is read-only.</span></span> <span data-ttu-id="b3261-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3261-152">createdDateTime</span></span>|<span data-ttu-id="b3261-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3261-153">DateTimeOffset</span></span>|<span data-ttu-id="b3261-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b3261-154">DateTime the object was created.</span></span> <span data-ttu-id="b3261-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-156">description</span><span class="sxs-lookup"><span data-stu-id="b3261-156">description</span></span>|<span data-ttu-id="b3261-157">String</span><span class="sxs-lookup"><span data-stu-id="b3261-157">String</span></span>|<span data-ttu-id="b3261-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3261-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3261-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b3261-160">displayName</span></span>|<span data-ttu-id="b3261-161">String</span><span class="sxs-lookup"><span data-stu-id="b3261-161">String</span></span>|<span data-ttu-id="b3261-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3261-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3261-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-164">version</span><span class="sxs-lookup"><span data-stu-id="b3261-164">version</span></span>|<span data-ttu-id="b3261-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b3261-165">Int32</span></span>|<span data-ttu-id="b3261-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3261-166">Version of the device configuration.</span></span> <span data-ttu-id="b3261-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3261-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b3261-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b3261-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b3261-169">Int32</span></span>|<span data-ttu-id="b3261-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3261-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b3261-171">Допустимые значения от 1 до 99 унаследованные от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b3261-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b3261-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b3261-172">subjectNameFormat</span></span>|[<span data-ttu-id="b3261-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b3261-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b3261-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3261-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b3261-175">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="b3261-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b3261-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b3261-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b3261-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b3261-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b3261-178">Int32</span></span>|<span data-ttu-id="b3261-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3261-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b3261-180">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b3261-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b3261-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b3261-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b3261-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b3261-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b3261-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3261-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b3261-184">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3261-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="b3261-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b3261-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b3261-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b3261-186">extendedKeyUsages</span></span>|<span data-ttu-id="b3261-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b3261-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b3261-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="b3261-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b3261-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b3261-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b3261-190">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b3261-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b3261-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b3261-191">certificationAuthority</span></span>|<span data-ttu-id="b3261-192">String</span><span class="sxs-lookup"><span data-stu-id="b3261-192">String</span></span>|<span data-ttu-id="b3261-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="b3261-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b3261-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b3261-194">certificationAuthorityName</span></span>|<span data-ttu-id="b3261-195">String</span><span class="sxs-lookup"><span data-stu-id="b3261-195">String</span></span>|<span data-ttu-id="b3261-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="b3261-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b3261-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b3261-197">certificateTemplateName</span></span>|<span data-ttu-id="b3261-198">String</span><span class="sxs-lookup"><span data-stu-id="b3261-198">String</span></span>|<span data-ttu-id="b3261-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="b3261-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b3261-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b3261-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b3261-201">String</span><span class="sxs-lookup"><span data-stu-id="b3261-201">String</span></span>|<span data-ttu-id="b3261-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="b3261-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b3261-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b3261-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b3261-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b3261-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b3261-205">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b3261-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b3261-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b3261-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="b3261-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3261-207">Response</span></span>
<span data-ttu-id="b3261-208">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3261-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3261-209">Пример</span><span class="sxs-lookup"><span data-stu-id="b3261-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3261-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3261-210">Request</span></span>
<span data-ttu-id="b3261-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3261-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="b3261-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3261-212">Response</span></span>
<span data-ttu-id="b3261-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b3261-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```




