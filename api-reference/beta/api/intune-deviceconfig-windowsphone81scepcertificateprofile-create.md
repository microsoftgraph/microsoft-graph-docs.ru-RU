---
title: Создание windowsPhone81SCEPCertificateProfile
description: Создание нового объекта windowsPhone81SCEPCertificateProfile.
author: tfitzmac
ms.openlocfilehash: b7c274f6e15578863d88f71900f815599ae420b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314093"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="b8928-103">Создание windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b8928-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="b8928-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8928-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8928-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8928-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8928-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8928-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8928-107">Создание нового объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b8928-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8928-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8928-108">Prerequisites</span></span>
<span data-ttu-id="b8928-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8928-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8928-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8928-111">Permission type</span></span>|<span data-ttu-id="b8928-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8928-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8928-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8928-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8928-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8928-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8928-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8928-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8928-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8928-116">Not supported.</span></span>|
|<span data-ttu-id="b8928-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8928-117">Application</span></span>|<span data-ttu-id="b8928-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8928-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8928-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8928-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8928-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8928-120">Request headers</span></span>
|<span data-ttu-id="b8928-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8928-121">Header</span></span>|<span data-ttu-id="b8928-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8928-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8928-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8928-123">Authorization</span></span>|<span data-ttu-id="b8928-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b8928-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8928-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8928-125">Accept</span></span>|<span data-ttu-id="b8928-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8928-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8928-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8928-127">Request body</span></span>
<span data-ttu-id="b8928-128">В тексте запроса укажите представление JSON для объекта windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b8928-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="b8928-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b8928-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="b8928-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8928-130">Property</span></span>|<span data-ttu-id="b8928-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b8928-131">Type</span></span>|<span data-ttu-id="b8928-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b8928-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8928-133">id</span><span class="sxs-lookup"><span data-stu-id="b8928-133">id</span></span>|<span data-ttu-id="b8928-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b8928-134">String</span></span>|<span data-ttu-id="b8928-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b8928-135">Key of the entity.</span></span> <span data-ttu-id="b8928-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8928-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8928-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8928-138">DateTimeOffset</span></span>|<span data-ttu-id="b8928-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b8928-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8928-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8928-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8928-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b8928-142">String collection</span></span>|<span data-ttu-id="b8928-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b8928-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8928-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8928-145">supportsScopeTags</span></span>|<span data-ttu-id="b8928-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b8928-146">Boolean</span></span>|<span data-ttu-id="b8928-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="b8928-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8928-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="b8928-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8928-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b8928-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8928-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8928-150">This property is read-only.</span></span> <span data-ttu-id="b8928-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8928-152">createdDateTime</span></span>|<span data-ttu-id="b8928-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8928-153">DateTimeOffset</span></span>|<span data-ttu-id="b8928-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b8928-154">DateTime the object was created.</span></span> <span data-ttu-id="b8928-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-156">описание</span><span class="sxs-lookup"><span data-stu-id="b8928-156">description</span></span>|<span data-ttu-id="b8928-157">Строка</span><span class="sxs-lookup"><span data-stu-id="b8928-157">String</span></span>|<span data-ttu-id="b8928-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8928-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8928-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b8928-160">displayName</span></span>|<span data-ttu-id="b8928-161">Строка</span><span class="sxs-lookup"><span data-stu-id="b8928-161">String</span></span>|<span data-ttu-id="b8928-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8928-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8928-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-164">version</span><span class="sxs-lookup"><span data-stu-id="b8928-164">version</span></span>|<span data-ttu-id="b8928-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b8928-165">Int32</span></span>|<span data-ttu-id="b8928-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8928-166">Version of the device configuration.</span></span> <span data-ttu-id="b8928-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8928-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b8928-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b8928-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b8928-169">Int32</span></span>|<span data-ttu-id="b8928-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8928-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b8928-171">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8928-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8928-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="b8928-172">keyStorageProvider</span></span>|[<span data-ttu-id="b8928-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="b8928-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="b8928-174">Поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="b8928-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="b8928-175">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="b8928-176">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b8928-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b8928-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b8928-177">subjectNameFormat</span></span>|[<span data-ttu-id="b8928-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b8928-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b8928-179">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8928-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="b8928-180">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="b8928-181">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b8928-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b8928-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b8928-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b8928-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b8928-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b8928-184">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8928-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b8928-185">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="b8928-186">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b8928-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b8928-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b8928-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b8928-188">Int32</span><span class="sxs-lookup"><span data-stu-id="b8928-188">Int32</span></span>|<span data-ttu-id="b8928-189">Значение периода Validtiy сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8928-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="b8928-190">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8928-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8928-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b8928-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b8928-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b8928-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b8928-193">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8928-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b8928-194">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b8928-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="b8928-195">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b8928-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b8928-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b8928-196">extendedKeyUsages</span></span>|<span data-ttu-id="b8928-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b8928-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b8928-198">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="b8928-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b8928-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b8928-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b8928-200">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8928-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8928-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b8928-201">scepServerUrls</span></span>|<span data-ttu-id="b8928-202">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b8928-202">String collection</span></span>|<span data-ttu-id="b8928-203">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8928-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="b8928-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b8928-204">subjectNameFormatString</span></span>|<span data-ttu-id="b8928-205">String.</span><span class="sxs-lookup"><span data-stu-id="b8928-205">String</span></span>|<span data-ttu-id="b8928-206">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="b8928-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b8928-207">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="b8928-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b8928-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="b8928-208">keyUsage</span></span>|[<span data-ttu-id="b8928-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b8928-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b8928-210">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="b8928-210">SCEP Key Usage.</span></span> <span data-ttu-id="b8928-211">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b8928-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b8928-212">keySize</span><span class="sxs-lookup"><span data-stu-id="b8928-212">keySize</span></span>|[<span data-ttu-id="b8928-213">keySize</span><span class="sxs-lookup"><span data-stu-id="b8928-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b8928-214">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8928-214">SCEP Key Size.</span></span> <span data-ttu-id="b8928-215">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="b8928-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b8928-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b8928-216">hashAlgorithm</span></span>|[<span data-ttu-id="b8928-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="b8928-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="b8928-218">Алгоритм хэширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8928-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="b8928-219">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="b8928-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="b8928-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b8928-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b8928-221">String.</span><span class="sxs-lookup"><span data-stu-id="b8928-221">String</span></span>|<span data-ttu-id="b8928-222">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="b8928-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="b8928-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8928-223">Response</span></span>
<span data-ttu-id="b8928-224">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b8928-224">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8928-225">Пример</span><span class="sxs-lookup"><span data-stu-id="b8928-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8928-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8928-226">Request</span></span>
<span data-ttu-id="b8928-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8928-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1096

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="b8928-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8928-228">Response</span></span>
<span data-ttu-id="b8928-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b8928-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





