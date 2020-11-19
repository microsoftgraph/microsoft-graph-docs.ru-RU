---
title: Создание windows10XSCEPCertificateProfile
description: Создание нового объекта windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d6fae55ffb8f97ab12eda59f4ac5b2d066e9f59
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242428"
---
# <a name="create-windows10xscepcertificateprofile"></a><span data-ttu-id="9f732-103">Создание windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9f732-103">Create windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="9f732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f732-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f732-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f732-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f732-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f732-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f732-107">Создание нового объекта [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9f732-107">Create a new [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f732-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f732-108">Prerequisites</span></span>
<span data-ttu-id="9f732-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f732-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f732-111">Permission type</span></span>|<span data-ttu-id="9f732-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f732-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f732-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f732-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f732-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f732-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f732-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f732-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f732-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f732-116">Not supported.</span></span>|
|<span data-ttu-id="9f732-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f732-117">Application</span></span>|<span data-ttu-id="9f732-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f732-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f732-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f732-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9f732-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f732-120">Request headers</span></span>
|<span data-ttu-id="9f732-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f732-121">Header</span></span>|<span data-ttu-id="9f732-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f732-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f732-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f732-123">Authorization</span></span>|<span data-ttu-id="9f732-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f732-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f732-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f732-125">Accept</span></span>|<span data-ttu-id="9f732-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f732-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f732-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f732-127">Request body</span></span>
<span data-ttu-id="9f732-128">В тексте запроса добавьте представление объекта windows10XSCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f732-128">In the request body, supply a JSON representation for the windows10XSCEPCertificateProfile object.</span></span>

<span data-ttu-id="9f732-129">В следующей таблице приведены свойства, необходимые при создании windows10XSCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="9f732-129">The following table shows the properties that are required when you create the windows10XSCEPCertificateProfile.</span></span>

|<span data-ttu-id="9f732-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f732-130">Property</span></span>|<span data-ttu-id="9f732-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f732-131">Type</span></span>|<span data-ttu-id="9f732-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f732-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f732-133">id</span><span class="sxs-lookup"><span data-stu-id="9f732-133">id</span></span>|<span data-ttu-id="9f732-134">String</span><span class="sxs-lookup"><span data-stu-id="9f732-134">String</span></span>|<span data-ttu-id="9f732-135">Идентификатор профиля унаследован от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-136">version</span><span class="sxs-lookup"><span data-stu-id="9f732-136">version</span></span>|<span data-ttu-id="9f732-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9f732-137">Int32</span></span>|<span data-ttu-id="9f732-138">Версия профиля, унаследованного от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9f732-139">displayName</span></span>|<span data-ttu-id="9f732-140">String</span><span class="sxs-lookup"><span data-stu-id="9f732-140">String</span></span>|<span data-ttu-id="9f732-141">Отображаемое имя профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-142">description</span><span class="sxs-lookup"><span data-stu-id="9f732-142">description</span></span>|<span data-ttu-id="9f732-143">String</span><span class="sxs-lookup"><span data-stu-id="9f732-143">String</span></span>|<span data-ttu-id="9f732-144">Описание профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-145">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="9f732-145">creationDateTime</span></span>|<span data-ttu-id="9f732-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f732-146">DateTimeOffset</span></span>|<span data-ttu-id="9f732-147">Создан профиль DateTime, наследуемый от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f732-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9f732-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f732-149">DateTimeOffset</span></span>|<span data-ttu-id="9f732-150">Последнее изменение профиля DateTime унаследовано от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f732-151">roleScopeTagIds</span></span>|<span data-ttu-id="9f732-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f732-152">String collection</span></span>|<span data-ttu-id="9f732-153">Теги областей унаследованы от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="9f732-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9f732-154">certificateStore</span></span>|[<span data-ttu-id="9f732-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9f732-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="9f732-156">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="9f732-156">Target store certificate.</span></span> <span data-ttu-id="9f732-157">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="9f732-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9f732-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f732-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9f732-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f732-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="9f732-160">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9f732-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9f732-161">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9f732-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9f732-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9f732-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9f732-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9f732-163">Int32</span></span>|<span data-ttu-id="9f732-164">Значение срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="9f732-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="9f732-165">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="9f732-165">extendedKeyUsages</span></span>|<span data-ttu-id="9f732-166">Коллекция [екстендедкэйусаже](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9f732-167">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="9f732-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="9f732-168">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="9f732-168">hashAlgorithm</span></span>|<span data-ttu-id="9f732-169">Коллекция [хашалгорисмс](../resources/intune-shared-hashalgorithms.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="9f732-170">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="9f732-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="9f732-171">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="9f732-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="9f732-172">keySize</span><span class="sxs-lookup"><span data-stu-id="9f732-172">keySize</span></span>|[<span data-ttu-id="9f732-173">keySize</span><span class="sxs-lookup"><span data-stu-id="9f732-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="9f732-174">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="9f732-174">SCEP Key Size.</span></span> <span data-ttu-id="9f732-175">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="9f732-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="9f732-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="9f732-176">keyStorageProvider</span></span>|[<span data-ttu-id="9f732-177">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="9f732-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="9f732-178">Поставщик хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="9f732-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="9f732-179">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="9f732-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="9f732-180">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="9f732-180">keyUsage</span></span>|[<span data-ttu-id="9f732-181">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="9f732-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="9f732-182">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="9f732-182">SCEP Key Usage.</span></span> <span data-ttu-id="9f732-183">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="9f732-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="9f732-184">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="9f732-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="9f732-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9f732-185">Int32</span></span>|<span data-ttu-id="9f732-186">Процент порогового возобновления сертификата</span><span class="sxs-lookup"><span data-stu-id="9f732-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="9f732-187">рутцертификатеид</span><span class="sxs-lookup"><span data-stu-id="9f732-187">rootCertificateId</span></span>|<span data-ttu-id="9f732-188">Guid</span><span class="sxs-lookup"><span data-stu-id="9f732-188">Guid</span></span>|<span data-ttu-id="9f732-189">ИД доверенного корневого сертификата</span><span class="sxs-lookup"><span data-stu-id="9f732-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="9f732-190">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="9f732-190">scepServerUrls</span></span>|<span data-ttu-id="9f732-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f732-191">String collection</span></span>|<span data-ttu-id="9f732-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="9f732-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="9f732-193">субжекталтернативенамеформатс</span><span class="sxs-lookup"><span data-stu-id="9f732-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="9f732-194">Коллекция [windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="9f732-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="9f732-195">Настраиваемые атрибуты AAD.</span><span class="sxs-lookup"><span data-stu-id="9f732-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="9f732-196">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="9f732-196">subjectNameFormatString</span></span>|<span data-ttu-id="9f732-197">String</span><span class="sxs-lookup"><span data-stu-id="9f732-197">String</span></span>|<span data-ttu-id="9f732-198">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="9f732-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="9f732-199">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="9f732-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="9f732-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f732-200">Response</span></span>
<span data-ttu-id="9f732-201">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f732-201">If successful, this method returns a `201 Created` response code and a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f732-202">Пример</span><span class="sxs-lookup"><span data-stu-id="9f732-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f732-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f732-203">Request</span></span>
<span data-ttu-id="9f732-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f732-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
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

### <a name="response"></a><span data-ttu-id="9f732-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f732-205">Response</span></span>
<span data-ttu-id="9f732-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f732-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




