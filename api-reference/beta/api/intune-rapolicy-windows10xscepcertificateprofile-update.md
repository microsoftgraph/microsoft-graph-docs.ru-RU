---
title: Обновление windows10XSCEPCertificateProfile
description: Обновление свойств объекта Windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 721b41e592d5885596efc185cfc1d2c5df2bcb2c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151923"
---
# <a name="update-windows10xscepcertificateprofile"></a><span data-ttu-id="9fea0-103">Обновление windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9fea0-103">Update windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="9fea0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fea0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fea0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fea0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fea0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fea0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fea0-107">Обновление свойств объекта [Windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-107">Update the properties of a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fea0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9fea0-108">Prerequisites</span></span>
<span data-ttu-id="9fea0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fea0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fea0-111">Permission type</span></span>|<span data-ttu-id="9fea0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fea0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fea0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fea0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fea0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fea0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9fea0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fea0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fea0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fea0-116">Not supported.</span></span>|
|<span data-ttu-id="9fea0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9fea0-117">Application</span></span>|<span data-ttu-id="9fea0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fea0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fea0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fea0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="9fea0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fea0-120">Request headers</span></span>
|<span data-ttu-id="9fea0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fea0-121">Header</span></span>|<span data-ttu-id="9fea0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9fea0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fea0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fea0-123">Authorization</span></span>|<span data-ttu-id="9fea0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fea0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fea0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fea0-125">Accept</span></span>|<span data-ttu-id="9fea0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fea0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fea0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fea0-127">Request body</span></span>
<span data-ttu-id="9fea0-128">В теле запроса поставляем представление JSON для [объекта Windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-128">In the request body, supply a JSON representation for the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="9fea0-129">В следующей таблице показаны свойства, необходимые при создании [windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-129">The following table shows the properties that are required when you create the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).</span></span>

|<span data-ttu-id="9fea0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fea0-130">Property</span></span>|<span data-ttu-id="9fea0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9fea0-131">Type</span></span>|<span data-ttu-id="9fea0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9fea0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fea0-133">id</span><span class="sxs-lookup"><span data-stu-id="9fea0-133">id</span></span>|<span data-ttu-id="9fea0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9fea0-134">String</span></span>|<span data-ttu-id="9fea0-135">Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-136">version</span><span class="sxs-lookup"><span data-stu-id="9fea0-136">version</span></span>|<span data-ttu-id="9fea0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9fea0-137">Int32</span></span>|<span data-ttu-id="9fea0-138">Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9fea0-139">displayName</span></span>|<span data-ttu-id="9fea0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="9fea0-140">String</span></span>|<span data-ttu-id="9fea0-141">Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-142">description</span><span class="sxs-lookup"><span data-stu-id="9fea0-142">description</span></span>|<span data-ttu-id="9fea0-143">Строка</span><span class="sxs-lookup"><span data-stu-id="9fea0-143">String</span></span>|<span data-ttu-id="9fea0-144">Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9fea0-145">creationDateTime</span></span>|<span data-ttu-id="9fea0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fea0-146">DateTimeOffset</span></span>|<span data-ttu-id="9fea0-147">Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fea0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9fea0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fea0-149">DateTimeOffset</span></span>|<span data-ttu-id="9fea0-150">Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fea0-151">roleScopeTagIds</span></span>|<span data-ttu-id="9fea0-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9fea0-152">String collection</span></span>|<span data-ttu-id="9fea0-153">Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9fea0-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9fea0-154">certificateStore</span></span>|[<span data-ttu-id="9fea0-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9fea0-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="9fea0-156">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="9fea0-156">Target store certificate.</span></span> <span data-ttu-id="9fea0-157">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9fea0-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9fea0-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9fea0-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9fea0-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="9fea0-160">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9fea0-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9fea0-161">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9fea0-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9fea0-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9fea0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9fea0-163">Int32</span></span>|<span data-ttu-id="9fea0-164">Значение для срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="9fea0-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="9fea0-165">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9fea0-165">extendedKeyUsages</span></span>|<span data-ttu-id="9fea0-166">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9fea0-167">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="9fea0-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="9fea0-168">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="9fea0-168">hashAlgorithm</span></span>|<span data-ttu-id="9fea0-169">[коллекция hashAlgorithms](../resources/intune-shared-hashalgorithms.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="9fea0-170">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="9fea0-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="9fea0-171">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="9fea0-172">keySize</span><span class="sxs-lookup"><span data-stu-id="9fea0-172">keySize</span></span>|[<span data-ttu-id="9fea0-173">keySize</span><span class="sxs-lookup"><span data-stu-id="9fea0-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="9fea0-174">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="9fea0-174">SCEP Key Size.</span></span> <span data-ttu-id="9fea0-175">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="9fea0-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="9fea0-176">keyStorageProvider</span></span>|[<span data-ttu-id="9fea0-177">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="9fea0-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="9fea0-178">Поставщик ключей для хранения данных (KSP).</span><span class="sxs-lookup"><span data-stu-id="9fea0-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="9fea0-179">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="9fea0-180">keyUsage</span><span class="sxs-lookup"><span data-stu-id="9fea0-180">keyUsage</span></span>|[<span data-ttu-id="9fea0-181">keyUsages</span><span class="sxs-lookup"><span data-stu-id="9fea0-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="9fea0-182">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="9fea0-182">SCEP Key Usage.</span></span> <span data-ttu-id="9fea0-183">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="9fea0-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="9fea0-184">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9fea0-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="9fea0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9fea0-185">Int32</span></span>|<span data-ttu-id="9fea0-186">Процент порогового значения обновления сертификата</span><span class="sxs-lookup"><span data-stu-id="9fea0-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="9fea0-187">rootCertificateId</span><span class="sxs-lookup"><span data-stu-id="9fea0-187">rootCertificateId</span></span>|<span data-ttu-id="9fea0-188">Guid</span><span class="sxs-lookup"><span data-stu-id="9fea0-188">Guid</span></span>|<span data-ttu-id="9fea0-189">Удостоверение доверенного корневого сертификата</span><span class="sxs-lookup"><span data-stu-id="9fea0-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="9fea0-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="9fea0-190">scepServerUrls</span></span>|<span data-ttu-id="9fea0-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9fea0-191">String collection</span></span>|<span data-ttu-id="9fea0-192">URL-адрес сервера SCEP Server (s).</span><span class="sxs-lookup"><span data-stu-id="9fea0-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="9fea0-193">subjectAlternativeNameFormats</span><span class="sxs-lookup"><span data-stu-id="9fea0-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="9fea0-194">[коллекция windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="9fea0-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="9fea0-195">Настраиваемые атрибуты AAD.</span><span class="sxs-lookup"><span data-stu-id="9fea0-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="9fea0-196">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9fea0-196">subjectNameFormatString</span></span>|<span data-ttu-id="9fea0-197">Строка</span><span class="sxs-lookup"><span data-stu-id="9fea0-197">String</span></span>|<span data-ttu-id="9fea0-198">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="9fea0-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="9fea0-199">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="9fea0-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="9fea0-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fea0-200">Response</span></span>
<span data-ttu-id="9fea0-201">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект Windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9fea0-201">If successful, this method returns a `200 OK` response code and an updated [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fea0-202">Пример</span><span class="sxs-lookup"><span data-stu-id="9fea0-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fea0-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fea0-203">Request</span></span>
<span data-ttu-id="9fea0-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fea0-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
Content-type: application/json
Content-length: 1178

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="9fea0-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fea0-205">Response</span></span>
<span data-ttu-id="9fea0-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fea0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1291

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```




