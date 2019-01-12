---
title: Создание androidWorkProfilePkcsCertificateProfile
description: Создание нового объекта androidWorkProfilePkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28cdeb6a2e87d91333a43fd97c14ac47d5d51659
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979756"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="2cc2b-103">Создание androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2cc2b-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="2cc2b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cc2b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cc2b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cc2b-107">Создание нового объекта [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2cc2b-107">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cc2b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2cc2b-108">Prerequisites</span></span>
<span data-ttu-id="2cc2b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc2b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc2b-111">Permission type</span></span>|<span data-ttu-id="2cc2b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc2b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc2b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc2b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc2b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc2b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-116">Not supported.</span></span>|
|<span data-ttu-id="2cc2b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cc2b-117">Application</span></span>|<span data-ttu-id="2cc2b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc2b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cc2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2cc2b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cc2b-120">Request headers</span></span>
|<span data-ttu-id="2cc2b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cc2b-121">Header</span></span>|<span data-ttu-id="2cc2b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cc2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc2b-123">Authorization</span></span>|<span data-ttu-id="2cc2b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2cc2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cc2b-125">Accept</span></span>|<span data-ttu-id="2cc2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc2b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cc2b-127">Request body</span></span>
<span data-ttu-id="2cc2b-128">В тексте запроса укажите представление JSON для объекта androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-128">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="2cc2b-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-129">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="2cc2b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cc2b-130">Property</span></span>|<span data-ttu-id="2cc2b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2cc2b-131">Type</span></span>|<span data-ttu-id="2cc2b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc2b-133">id</span><span class="sxs-lookup"><span data-stu-id="2cc2b-133">id</span></span>|<span data-ttu-id="2cc2b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-134">String</span></span>|<span data-ttu-id="2cc2b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-135">Key of the entity.</span></span> <span data-ttu-id="2cc2b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc2b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2cc2b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc2b-138">DateTimeOffset</span></span>|<span data-ttu-id="2cc2b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2cc2b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2cc2b-141">roleScopeTagIds</span></span>|<span data-ttu-id="2cc2b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2cc2b-142">String collection</span></span>|<span data-ttu-id="2cc2b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2cc2b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2cc2b-145">supportsScopeTags</span></span>|<span data-ttu-id="2cc2b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2cc2b-146">Boolean</span></span>|<span data-ttu-id="2cc2b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2cc2b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2cc2b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2cc2b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-150">This property is read-only.</span></span> <span data-ttu-id="2cc2b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc2b-152">createdDateTime</span></span>|<span data-ttu-id="2cc2b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc2b-153">DateTimeOffset</span></span>|<span data-ttu-id="2cc2b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-154">DateTime the object was created.</span></span> <span data-ttu-id="2cc2b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-156">описание</span><span class="sxs-lookup"><span data-stu-id="2cc2b-156">description</span></span>|<span data-ttu-id="2cc2b-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-157">String</span></span>|<span data-ttu-id="2cc2b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2cc2b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2cc2b-160">displayName</span></span>|<span data-ttu-id="2cc2b-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-161">String</span></span>|<span data-ttu-id="2cc2b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2cc2b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-164">version</span><span class="sxs-lookup"><span data-stu-id="2cc2b-164">version</span></span>|<span data-ttu-id="2cc2b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2cc2b-165">Int32</span></span>|<span data-ttu-id="2cc2b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-166">Version of the device configuration.</span></span> <span data-ttu-id="2cc2b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cc2b-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2cc2b-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="2cc2b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2cc2b-169">Int32</span></span>|<span data-ttu-id="2cc2b-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2cc2b-171">Допустимые значения от 1 до 99 унаследованные от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2cc2b-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2cc2b-172">subjectNameFormat</span></span>|[<span data-ttu-id="2cc2b-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2cc2b-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="2cc2b-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="2cc2b-175">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="2cc2b-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="2cc2b-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2cc2b-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2cc2b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="2cc2b-178">Int32</span></span>|<span data-ttu-id="2cc2b-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="2cc2b-180">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2cc2b-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2cc2b-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2cc2b-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2cc2b-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2cc2b-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2cc2b-184">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="2cc2b-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2cc2b-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2cc2b-186">extendedKeyUsages</span></span>|<span data-ttu-id="2cc2b-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2cc2b-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="2cc2b-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="2cc2b-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="2cc2b-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2cc2b-190">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2cc2b-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2cc2b-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="2cc2b-191">certificationAuthority</span></span>|<span data-ttu-id="2cc2b-192">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-192">String</span></span>|<span data-ttu-id="2cc2b-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="2cc2b-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="2cc2b-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="2cc2b-194">certificationAuthorityName</span></span>|<span data-ttu-id="2cc2b-195">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-195">String</span></span>|<span data-ttu-id="2cc2b-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="2cc2b-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="2cc2b-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="2cc2b-197">certificateTemplateName</span></span>|<span data-ttu-id="2cc2b-198">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-198">String</span></span>|<span data-ttu-id="2cc2b-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="2cc2b-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="2cc2b-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2cc2b-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="2cc2b-201">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc2b-201">String</span></span>|<span data-ttu-id="2cc2b-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="2cc2b-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2cc2b-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="2cc2b-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2cc2b-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2cc2b-205">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="2cc2b-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="2cc2b-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cc2b-207">Response</span></span>
<span data-ttu-id="2cc2b-208">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc2b-209">Пример</span><span class="sxs-lookup"><span data-stu-id="2cc2b-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cc2b-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cc2b-210">Request</span></span>
<span data-ttu-id="2cc2b-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1033

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="2cc2b-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cc2b-212">Response</span></span>
<span data-ttu-id="2cc2b-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2cc2b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





