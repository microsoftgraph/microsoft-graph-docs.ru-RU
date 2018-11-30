---
title: Обновление androidForWorkPkcsCertificateProfile
description: Обновление свойства объекта androidForWorkPkcsCertificateProfile.
ms.openlocfilehash: aa66069317ea2be9d13b21e8f909edc2a36ddc99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080579"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="039b1-103">Обновление androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="039b1-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="039b1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="039b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="039b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="039b1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="039b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="039b1-107">Обновление свойства объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="039b1-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="039b1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="039b1-108">Prerequisites</span></span>
<span data-ttu-id="039b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="039b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="039b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="039b1-111">Permission type</span></span>|<span data-ttu-id="039b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="039b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="039b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="039b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="039b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="039b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="039b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="039b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039b1-116">Not supported.</span></span>|
|<span data-ttu-id="039b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="039b1-117">Application</span></span>|<span data-ttu-id="039b1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="039b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="039b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="039b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="039b1-120">Request headers</span></span>
|<span data-ttu-id="039b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="039b1-121">Header</span></span>|<span data-ttu-id="039b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="039b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="039b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="039b1-123">Authorization</span></span>|<span data-ttu-id="039b1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="039b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="039b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="039b1-125">Accept</span></span>|<span data-ttu-id="039b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="039b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="039b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="039b1-127">Request body</span></span>
<span data-ttu-id="039b1-128">В тексте запроса укажите представление JSON для объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="039b1-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="039b1-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="039b1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="039b1-130">Property</span></span>|<span data-ttu-id="039b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="039b1-131">Type</span></span>|<span data-ttu-id="039b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="039b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039b1-133">id</span><span class="sxs-lookup"><span data-stu-id="039b1-133">id</span></span>|<span data-ttu-id="039b1-134">String</span><span class="sxs-lookup"><span data-stu-id="039b1-134">String</span></span>|<span data-ttu-id="039b1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="039b1-135">Key of the entity.</span></span> <span data-ttu-id="039b1-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="039b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="039b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039b1-138">DateTimeOffset</span></span>|<span data-ttu-id="039b1-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="039b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="039b1-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="039b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="039b1-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="039b1-142">String collection</span></span>|<span data-ttu-id="039b1-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="039b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="039b1-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="039b1-145">supportsScopeTags</span></span>|<span data-ttu-id="039b1-146">Логический</span><span class="sxs-lookup"><span data-stu-id="039b1-146">Boolean</span></span>|<span data-ttu-id="039b1-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="039b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="039b1-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="039b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="039b1-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="039b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="039b1-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="039b1-150">This property is read-only.</span></span> <span data-ttu-id="039b1-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="039b1-152">createdDateTime</span></span>|<span data-ttu-id="039b1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039b1-153">DateTimeOffset</span></span>|<span data-ttu-id="039b1-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="039b1-154">DateTime the object was created.</span></span> <span data-ttu-id="039b1-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-156">описание</span><span class="sxs-lookup"><span data-stu-id="039b1-156">description</span></span>|<span data-ttu-id="039b1-157">String</span><span class="sxs-lookup"><span data-stu-id="039b1-157">String</span></span>|<span data-ttu-id="039b1-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039b1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="039b1-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="039b1-160">displayName</span></span>|<span data-ttu-id="039b1-161">String</span><span class="sxs-lookup"><span data-stu-id="039b1-161">String</span></span>|<span data-ttu-id="039b1-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039b1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="039b1-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-164">version</span><span class="sxs-lookup"><span data-stu-id="039b1-164">version</span></span>|<span data-ttu-id="039b1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="039b1-165">Int32</span></span>|<span data-ttu-id="039b1-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039b1-166">Version of the device configuration.</span></span> <span data-ttu-id="039b1-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="039b1-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="039b1-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="039b1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="039b1-169">Int32</span></span>|<span data-ttu-id="039b1-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="039b1-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="039b1-171">Допустимые значения от 1 до 99 унаследованные от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="039b1-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="039b1-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="039b1-172">subjectNameFormat</span></span>|[<span data-ttu-id="039b1-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="039b1-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="039b1-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="039b1-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="039b1-175">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="039b1-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="039b1-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="039b1-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="039b1-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="039b1-178">Int32</span><span class="sxs-lookup"><span data-stu-id="039b1-178">Int32</span></span>|<span data-ttu-id="039b1-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="039b1-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="039b1-180">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="039b1-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="039b1-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="039b1-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="039b1-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="039b1-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="039b1-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="039b1-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="039b1-184">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="039b1-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="039b1-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="039b1-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="039b1-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="039b1-186">extendedKeyUsages</span></span>|<span data-ttu-id="039b1-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="039b1-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="039b1-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="039b1-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="039b1-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="039b1-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="039b1-190">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="039b1-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="039b1-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="039b1-191">certificationAuthority</span></span>|<span data-ttu-id="039b1-192">String</span><span class="sxs-lookup"><span data-stu-id="039b1-192">String</span></span>|<span data-ttu-id="039b1-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="039b1-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="039b1-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="039b1-194">certificationAuthorityName</span></span>|<span data-ttu-id="039b1-195">String</span><span class="sxs-lookup"><span data-stu-id="039b1-195">String</span></span>|<span data-ttu-id="039b1-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="039b1-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="039b1-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="039b1-197">certificateTemplateName</span></span>|<span data-ttu-id="039b1-198">String</span><span class="sxs-lookup"><span data-stu-id="039b1-198">String</span></span>|<span data-ttu-id="039b1-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="039b1-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="039b1-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="039b1-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="039b1-201">String</span><span class="sxs-lookup"><span data-stu-id="039b1-201">String</span></span>|<span data-ttu-id="039b1-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="039b1-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="039b1-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="039b1-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="039b1-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="039b1-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="039b1-205">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="039b1-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="039b1-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="039b1-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="039b1-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="039b1-207">Response</span></span>
<span data-ttu-id="039b1-208">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="039b1-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039b1-209">Пример</span><span class="sxs-lookup"><span data-stu-id="039b1-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="039b1-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="039b1-210">Request</span></span>
<span data-ttu-id="039b1-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="039b1-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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

### <a name="response"></a><span data-ttu-id="039b1-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="039b1-212">Response</span></span>
<span data-ttu-id="039b1-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="039b1-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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





