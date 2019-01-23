---
title: Создание androidScepCertificateProfile
description: Создание нового объекта androidScepCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1e208882f0524acd26e390b82a7624995603b42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425087"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="aae09-103">Создание androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="aae09-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="aae09-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aae09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aae09-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aae09-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aae09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aae09-107">Создание нового объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aae09-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aae09-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="aae09-108">Prerequisites</span></span>
<span data-ttu-id="aae09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aae09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aae09-111">Permission type</span></span>|<span data-ttu-id="aae09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aae09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aae09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aae09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aae09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aae09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aae09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aae09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae09-116">Not supported.</span></span>|
|<span data-ttu-id="aae09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aae09-117">Application</span></span>|<span data-ttu-id="aae09-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae09-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aae09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aae09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aae09-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aae09-120">Request headers</span></span>
|<span data-ttu-id="aae09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aae09-121">Header</span></span>|<span data-ttu-id="aae09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aae09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aae09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aae09-123">Authorization</span></span>|<span data-ttu-id="aae09-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aae09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aae09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aae09-125">Accept</span></span>|<span data-ttu-id="aae09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aae09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aae09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aae09-127">Request body</span></span>
<span data-ttu-id="aae09-128">В тексте запроса укажите представление JSON для объекта androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="aae09-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="aae09-129">В следующей таблице показаны свойства, которые необходимы для создания androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="aae09-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="aae09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aae09-130">Property</span></span>|<span data-ttu-id="aae09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aae09-131">Type</span></span>|<span data-ttu-id="aae09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aae09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae09-133">id</span><span class="sxs-lookup"><span data-stu-id="aae09-133">id</span></span>|<span data-ttu-id="aae09-134">String</span><span class="sxs-lookup"><span data-stu-id="aae09-134">String</span></span>|<span data-ttu-id="aae09-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aae09-135">Key of the entity.</span></span> <span data-ttu-id="aae09-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae09-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aae09-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae09-138">DateTimeOffset</span></span>|<span data-ttu-id="aae09-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aae09-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aae09-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aae09-141">roleScopeTagIds</span></span>|<span data-ttu-id="aae09-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aae09-142">String collection</span></span>|<span data-ttu-id="aae09-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aae09-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aae09-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aae09-145">supportsScopeTags</span></span>|<span data-ttu-id="aae09-146">Логический</span><span class="sxs-lookup"><span data-stu-id="aae09-146">Boolean</span></span>|<span data-ttu-id="aae09-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="aae09-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aae09-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="aae09-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aae09-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aae09-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aae09-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae09-150">This property is read-only.</span></span> <span data-ttu-id="aae09-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aae09-152">createdDateTime</span></span>|<span data-ttu-id="aae09-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae09-153">DateTimeOffset</span></span>|<span data-ttu-id="aae09-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aae09-154">DateTime the object was created.</span></span> <span data-ttu-id="aae09-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-156">description</span><span class="sxs-lookup"><span data-stu-id="aae09-156">description</span></span>|<span data-ttu-id="aae09-157">String</span><span class="sxs-lookup"><span data-stu-id="aae09-157">String</span></span>|<span data-ttu-id="aae09-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aae09-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aae09-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-160">displayName</span><span class="sxs-lookup"><span data-stu-id="aae09-160">displayName</span></span>|<span data-ttu-id="aae09-161">String</span><span class="sxs-lookup"><span data-stu-id="aae09-161">String</span></span>|<span data-ttu-id="aae09-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aae09-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aae09-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-164">version</span><span class="sxs-lookup"><span data-stu-id="aae09-164">version</span></span>|<span data-ttu-id="aae09-165">Int32</span><span class="sxs-lookup"><span data-stu-id="aae09-165">Int32</span></span>|<span data-ttu-id="aae09-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aae09-166">Version of the device configuration.</span></span> <span data-ttu-id="aae09-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aae09-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="aae09-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="aae09-169">Int32</span><span class="sxs-lookup"><span data-stu-id="aae09-169">Int32</span></span>|<span data-ttu-id="aae09-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="aae09-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="aae09-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="aae09-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="aae09-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="aae09-172">subjectNameFormat</span></span>|[<span data-ttu-id="aae09-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="aae09-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="aae09-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="aae09-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="aae09-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="aae09-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="aae09-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="aae09-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="aae09-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="aae09-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="aae09-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="aae09-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="aae09-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="aae09-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="aae09-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="aae09-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="aae09-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="aae09-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="aae09-183">Int32</span><span class="sxs-lookup"><span data-stu-id="aae09-183">Int32</span></span>|<span data-ttu-id="aae09-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="aae09-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="aae09-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="aae09-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="aae09-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="aae09-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="aae09-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="aae09-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="aae09-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="aae09-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="aae09-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="aae09-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="aae09-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="aae09-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="aae09-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="aae09-191">extendedKeyUsages</span></span>|<span data-ttu-id="aae09-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="aae09-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="aae09-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="aae09-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="aae09-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aae09-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="aae09-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="aae09-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="aae09-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="aae09-196">scepServerUrls</span></span>|<span data-ttu-id="aae09-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aae09-197">String collection</span></span>|<span data-ttu-id="aae09-198">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="aae09-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="aae09-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="aae09-199">subjectNameFormatString</span></span>|<span data-ttu-id="aae09-200">String</span><span class="sxs-lookup"><span data-stu-id="aae09-200">String</span></span>|<span data-ttu-id="aae09-201">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="aae09-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="aae09-202">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="aae09-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="aae09-203">keyUsage</span><span class="sxs-lookup"><span data-stu-id="aae09-203">keyUsage</span></span>|[<span data-ttu-id="aae09-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="aae09-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="aae09-205">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="aae09-205">SCEP Key Usage.</span></span> <span data-ttu-id="aae09-206">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="aae09-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="aae09-207">keySize</span><span class="sxs-lookup"><span data-stu-id="aae09-207">keySize</span></span>|[<span data-ttu-id="aae09-208">keySize</span><span class="sxs-lookup"><span data-stu-id="aae09-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="aae09-209">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="aae09-209">SCEP Key Size.</span></span> <span data-ttu-id="aae09-210">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="aae09-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="aae09-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="aae09-211">hashAlgorithm</span></span>|[<span data-ttu-id="aae09-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="aae09-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="aae09-213">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="aae09-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="aae09-214">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="aae09-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="aae09-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="aae09-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="aae09-216">String</span><span class="sxs-lookup"><span data-stu-id="aae09-216">String</span></span>|<span data-ttu-id="aae09-217">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="aae09-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="aae09-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae09-218">Response</span></span>
<span data-ttu-id="aae09-219">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aae09-219">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aae09-220">Пример</span><span class="sxs-lookup"><span data-stu-id="aae09-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="aae09-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="aae09-221">Request</span></span>
<span data-ttu-id="aae09-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aae09-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
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

### <a name="response"></a><span data-ttu-id="aae09-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae09-223">Response</span></span>
<span data-ttu-id="aae09-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aae09-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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




