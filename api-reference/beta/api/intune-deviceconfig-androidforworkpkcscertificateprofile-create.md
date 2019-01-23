---
title: Создание androidForWorkPkcsCertificateProfile
description: Создание нового объекта androidForWorkPkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6d00875bffec7405e4e5d955afe906572df5d36
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401098"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="6917a-103">Создание androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6917a-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="6917a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6917a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6917a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6917a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6917a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6917a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6917a-107">Создание нового объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6917a-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6917a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="6917a-108">Prerequisites</span></span>
<span data-ttu-id="6917a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6917a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6917a-111">Permission type</span></span>|<span data-ttu-id="6917a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6917a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6917a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6917a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6917a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6917a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6917a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6917a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6917a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6917a-116">Not supported.</span></span>|
|<span data-ttu-id="6917a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6917a-117">Application</span></span>|<span data-ttu-id="6917a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6917a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6917a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6917a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6917a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6917a-120">Request headers</span></span>
|<span data-ttu-id="6917a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6917a-121">Header</span></span>|<span data-ttu-id="6917a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6917a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6917a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6917a-123">Authorization</span></span>|<span data-ttu-id="6917a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6917a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6917a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6917a-125">Accept</span></span>|<span data-ttu-id="6917a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6917a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6917a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6917a-127">Request body</span></span>
<span data-ttu-id="6917a-128">В тексте запроса укажите представление JSON для объекта androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6917a-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="6917a-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6917a-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="6917a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6917a-130">Property</span></span>|<span data-ttu-id="6917a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6917a-131">Type</span></span>|<span data-ttu-id="6917a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6917a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6917a-133">id</span><span class="sxs-lookup"><span data-stu-id="6917a-133">id</span></span>|<span data-ttu-id="6917a-134">String</span><span class="sxs-lookup"><span data-stu-id="6917a-134">String</span></span>|<span data-ttu-id="6917a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6917a-135">Key of the entity.</span></span> <span data-ttu-id="6917a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6917a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6917a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6917a-138">DateTimeOffset</span></span>|<span data-ttu-id="6917a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6917a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6917a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6917a-141">roleScopeTagIds</span></span>|<span data-ttu-id="6917a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6917a-142">String collection</span></span>|<span data-ttu-id="6917a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6917a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6917a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6917a-145">supportsScopeTags</span></span>|<span data-ttu-id="6917a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6917a-146">Boolean</span></span>|<span data-ttu-id="6917a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6917a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6917a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6917a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6917a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6917a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6917a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6917a-150">This property is read-only.</span></span> <span data-ttu-id="6917a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6917a-152">createdDateTime</span></span>|<span data-ttu-id="6917a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6917a-153">DateTimeOffset</span></span>|<span data-ttu-id="6917a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6917a-154">DateTime the object was created.</span></span> <span data-ttu-id="6917a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-156">description</span><span class="sxs-lookup"><span data-stu-id="6917a-156">description</span></span>|<span data-ttu-id="6917a-157">String</span><span class="sxs-lookup"><span data-stu-id="6917a-157">String</span></span>|<span data-ttu-id="6917a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6917a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6917a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6917a-160">displayName</span></span>|<span data-ttu-id="6917a-161">String</span><span class="sxs-lookup"><span data-stu-id="6917a-161">String</span></span>|<span data-ttu-id="6917a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6917a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6917a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-164">version</span><span class="sxs-lookup"><span data-stu-id="6917a-164">version</span></span>|<span data-ttu-id="6917a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6917a-165">Int32</span></span>|<span data-ttu-id="6917a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6917a-166">Version of the device configuration.</span></span> <span data-ttu-id="6917a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6917a-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6917a-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6917a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6917a-169">Int32</span></span>|<span data-ttu-id="6917a-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="6917a-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6917a-171">Допустимые значения от 1 до 99 унаследованные от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6917a-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6917a-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6917a-172">subjectNameFormat</span></span>|[<span data-ttu-id="6917a-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6917a-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6917a-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="6917a-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="6917a-175">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6917a-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6917a-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6917a-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6917a-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6917a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6917a-178">Int32</span></span>|<span data-ttu-id="6917a-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="6917a-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6917a-180">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6917a-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6917a-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6917a-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6917a-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6917a-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6917a-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="6917a-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6917a-184">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6917a-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6917a-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6917a-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6917a-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6917a-186">extendedKeyUsages</span></span>|<span data-ttu-id="6917a-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6917a-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6917a-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="6917a-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6917a-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6917a-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6917a-190">Наследуется от [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6917a-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6917a-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="6917a-191">certificationAuthority</span></span>|<span data-ttu-id="6917a-192">String</span><span class="sxs-lookup"><span data-stu-id="6917a-192">String</span></span>|<span data-ttu-id="6917a-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="6917a-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="6917a-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="6917a-194">certificationAuthorityName</span></span>|<span data-ttu-id="6917a-195">String</span><span class="sxs-lookup"><span data-stu-id="6917a-195">String</span></span>|<span data-ttu-id="6917a-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="6917a-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="6917a-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="6917a-197">certificateTemplateName</span></span>|<span data-ttu-id="6917a-198">String</span><span class="sxs-lookup"><span data-stu-id="6917a-198">String</span></span>|<span data-ttu-id="6917a-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="6917a-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="6917a-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6917a-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6917a-201">String</span><span class="sxs-lookup"><span data-stu-id="6917a-201">String</span></span>|<span data-ttu-id="6917a-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="6917a-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="6917a-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6917a-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6917a-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6917a-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6917a-205">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="6917a-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6917a-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6917a-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="6917a-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="6917a-207">Response</span></span>
<span data-ttu-id="6917a-208">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6917a-208">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6917a-209">Пример</span><span class="sxs-lookup"><span data-stu-id="6917a-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="6917a-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="6917a-210">Request</span></span>
<span data-ttu-id="6917a-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6917a-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 965

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="6917a-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="6917a-212">Response</span></span>
<span data-ttu-id="6917a-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6917a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




