---
title: Создание Усерпфксцертификате
description: Создание нового объекта Усерпфксцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c979bb141166544f374dd3fb38b765e46d0bcba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460075"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="ee166-103">Создание Усерпфксцертификате</span><span class="sxs-lookup"><span data-stu-id="ee166-103">Create userPFXCertificate</span></span>

<span data-ttu-id="ee166-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee166-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee166-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee166-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee166-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee166-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee166-107">Создание нового объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ee166-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee166-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee166-108">Prerequisites</span></span>
<span data-ttu-id="ee166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee166-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee166-111">Permission type</span></span>|<span data-ttu-id="ee166-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee166-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee166-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee166-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee166-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee166-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee166-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee166-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee166-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee166-116">Not supported.</span></span>|
|<span data-ttu-id="ee166-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee166-117">Application</span></span>|<span data-ttu-id="ee166-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee166-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee166-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee166-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ee166-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee166-120">Request headers</span></span>
|<span data-ttu-id="ee166-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee166-121">Header</span></span>|<span data-ttu-id="ee166-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee166-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee166-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee166-123">Authorization</span></span>|<span data-ttu-id="ee166-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee166-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee166-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee166-125">Accept</span></span>|<span data-ttu-id="ee166-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee166-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee166-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee166-127">Request body</span></span>
<span data-ttu-id="ee166-128">В тексте запроса добавьте представление объекта Усерпфксцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee166-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="ee166-129">В следующей таблице приведены свойства, необходимые при создании Усерпфксцертификате.</span><span class="sxs-lookup"><span data-stu-id="ee166-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="ee166-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee166-130">Property</span></span>|<span data-ttu-id="ee166-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee166-131">Type</span></span>|<span data-ttu-id="ee166-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee166-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee166-133">id</span><span class="sxs-lookup"><span data-stu-id="ee166-133">id</span></span>|<span data-ttu-id="ee166-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ee166-134">String</span></span>|<span data-ttu-id="ee166-135">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="ee166-136">отпечаток</span><span class="sxs-lookup"><span data-stu-id="ee166-136">thumbprint</span></span>|<span data-ttu-id="ee166-137">String</span><span class="sxs-lookup"><span data-stu-id="ee166-137">String</span></span>|<span data-ttu-id="ee166-138">Отпечаток SHA-1 сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="ee166-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ee166-139">intendedPurpose</span></span>|[<span data-ttu-id="ee166-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ee166-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="ee166-141">Сертификат, предназначенный для целей из точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ee166-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="ee166-142">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="ee166-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="ee166-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee166-143">userPrincipalName</span></span>|<span data-ttu-id="ee166-144">String</span><span class="sxs-lookup"><span data-stu-id="ee166-144">String</span></span>|<span data-ttu-id="ee166-145">Имя участника-пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="ee166-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ee166-146">startDateTime</span></span>|<span data-ttu-id="ee166-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee166-147">DateTimeOffset</span></span>|<span data-ttu-id="ee166-148">Дата и время начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee166-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="ee166-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee166-149">expirationDateTime</span></span>|<span data-ttu-id="ee166-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee166-150">DateTimeOffset</span></span>|<span data-ttu-id="ee166-151">Дата и время действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee166-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="ee166-152">providerName</span><span class="sxs-lookup"><span data-stu-id="ee166-152">providerName</span></span>|<span data-ttu-id="ee166-153">String</span><span class="sxs-lookup"><span data-stu-id="ee166-153">String</span></span>|<span data-ttu-id="ee166-154">Поставщик криптографии, используемый для шифрования этого объекта BLOB.</span><span class="sxs-lookup"><span data-stu-id="ee166-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="ee166-155">keyName</span><span class="sxs-lookup"><span data-stu-id="ee166-155">keyName</span></span>|<span data-ttu-id="ee166-156">String</span><span class="sxs-lookup"><span data-stu-id="ee166-156">String</span></span>|<span data-ttu-id="ee166-157">Имя ключа (в пределах поставщика), используемого для шифрования большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ee166-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="ee166-158">паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="ee166-158">paddingScheme</span></span>|[<span data-ttu-id="ee166-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="ee166-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="ee166-160">Схема заполнения, используемая поставщиком во время шифрования и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="ee166-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="ee166-161">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="ee166-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="ee166-162">енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="ee166-162">encryptedPfxBlob</span></span>|<span data-ttu-id="ee166-163">Binary</span><span class="sxs-lookup"><span data-stu-id="ee166-163">Binary</span></span>|<span data-ttu-id="ee166-164">Зашифрованный BLOB-объект PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="ee166-165">енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="ee166-165">encryptedPfxPassword</span></span>|<span data-ttu-id="ee166-166">String</span><span class="sxs-lookup"><span data-stu-id="ee166-166">String</span></span>|<span data-ttu-id="ee166-167">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="ee166-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee166-168">createdDateTime</span></span>|<span data-ttu-id="ee166-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee166-169">DateTimeOffset</span></span>|<span data-ttu-id="ee166-170">Дата и время импорта этого PFX-сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee166-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="ee166-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee166-171">lastModifiedDateTime</span></span>|<span data-ttu-id="ee166-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee166-172">DateTimeOffset</span></span>|<span data-ttu-id="ee166-173">Дата и время последнего изменения сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="ee166-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ee166-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee166-174">Response</span></span>
<span data-ttu-id="ee166-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee166-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee166-176">Пример</span><span class="sxs-lookup"><span data-stu-id="ee166-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee166-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee166-177">Request</span></span>
<span data-ttu-id="ee166-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee166-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a><span data-ttu-id="ee166-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee166-179">Response</span></span>
<span data-ttu-id="ee166-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee166-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





