---
title: Создание Усерпфксцертификате
description: Создание нового объекта Усерпфксцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d71812bc1a4e41f01e8353b49a4e656613a8d2b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899734"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="0e3bc-103">Создание Усерпфксцертификате</span><span class="sxs-lookup"><span data-stu-id="0e3bc-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="0e3bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e3bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e3bc-106">Создание нового объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0e3bc-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e3bc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e3bc-107">Prerequisites</span></span>
<span data-ttu-id="0e3bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e3bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e3bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e3bc-110">Permission type</span></span>|<span data-ttu-id="0e3bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e3bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e3bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e3bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e3bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-115">Not supported.</span></span>|
|<span data-ttu-id="0e3bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e3bc-116">Application</span></span>|<span data-ttu-id="0e3bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e3bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="0e3bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e3bc-119">Request headers</span></span>
|<span data-ttu-id="0e3bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e3bc-120">Header</span></span>|<span data-ttu-id="0e3bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e3bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e3bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e3bc-122">Authorization</span></span>|<span data-ttu-id="0e3bc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e3bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e3bc-124">Accept</span></span>|<span data-ttu-id="0e3bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e3bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e3bc-126">Request body</span></span>
<span data-ttu-id="0e3bc-127">В тексте запроса добавьте представление объекта Усерпфксцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="0e3bc-128">В следующей таблице приведены свойства, необходимые при создании Усерпфксцертификате.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="0e3bc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e3bc-129">Property</span></span>|<span data-ttu-id="0e3bc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e3bc-130">Type</span></span>|<span data-ttu-id="0e3bc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e3bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e3bc-132">id</span><span class="sxs-lookup"><span data-stu-id="0e3bc-132">id</span></span>|<span data-ttu-id="0e3bc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3bc-133">String</span></span>|<span data-ttu-id="0e3bc-134">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="0e3bc-135">отпечаток</span><span class="sxs-lookup"><span data-stu-id="0e3bc-135">thumbprint</span></span>|<span data-ttu-id="0e3bc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3bc-136">String</span></span>|<span data-ttu-id="0e3bc-137">Отпечаток SHA-1 сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="0e3bc-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0e3bc-138">intendedPurpose</span></span>|[<span data-ttu-id="0e3bc-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0e3bc-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="0e3bc-140">Сертификат, предназначенный для целей из точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="0e3bc-141">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="0e3bc-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e3bc-142">userPrincipalName</span></span>|<span data-ttu-id="0e3bc-143">String</span><span class="sxs-lookup"><span data-stu-id="0e3bc-143">String</span></span>|<span data-ttu-id="0e3bc-144">Имя участника-пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="0e3bc-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bc-145">startDateTime</span></span>|<span data-ttu-id="0e3bc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bc-146">DateTimeOffset</span></span>|<span data-ttu-id="0e3bc-147">Дата и время начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="0e3bc-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bc-148">expirationDateTime</span></span>|<span data-ttu-id="0e3bc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bc-149">DateTimeOffset</span></span>|<span data-ttu-id="0e3bc-150">Дата и время действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="0e3bc-151">providerName</span><span class="sxs-lookup"><span data-stu-id="0e3bc-151">providerName</span></span>|<span data-ttu-id="0e3bc-152">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3bc-152">String</span></span>|<span data-ttu-id="0e3bc-153">Поставщик криптографии, используемый для шифрования этого объекта BLOB.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="0e3bc-154">keyName</span><span class="sxs-lookup"><span data-stu-id="0e3bc-154">keyName</span></span>|<span data-ttu-id="0e3bc-155">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3bc-155">String</span></span>|<span data-ttu-id="0e3bc-156">Имя ключа (в пределах поставщика), используемого для шифрования большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="0e3bc-157">Паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="0e3bc-157">paddingScheme</span></span>|[<span data-ttu-id="0e3bc-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="0e3bc-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="0e3bc-159">Схема заполнения, используемая поставщиком во время шифрования и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="0e3bc-160">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="0e3bc-161">Енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="0e3bc-161">encryptedPfxBlob</span></span>|<span data-ttu-id="0e3bc-162">Binary</span><span class="sxs-lookup"><span data-stu-id="0e3bc-162">Binary</span></span>|<span data-ttu-id="0e3bc-163">Зашифрованный BLOB-объект PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="0e3bc-164">Енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="0e3bc-164">encryptedPfxPassword</span></span>|<span data-ttu-id="0e3bc-165">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3bc-165">String</span></span>|<span data-ttu-id="0e3bc-166">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="0e3bc-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bc-167">createdDateTime</span></span>|<span data-ttu-id="0e3bc-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bc-168">DateTimeOffset</span></span>|<span data-ttu-id="0e3bc-169">Дата и время импорта этого PFX-сертификата.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="0e3bc-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bc-170">lastModifiedDateTime</span></span>|<span data-ttu-id="0e3bc-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bc-171">DateTimeOffset</span></span>|<span data-ttu-id="0e3bc-172">Дата и время последнего изменения сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0e3bc-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3bc-173">Response</span></span>
<span data-ttu-id="0e3bc-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3bc-175">Пример</span><span class="sxs-lookup"><span data-stu-id="0e3bc-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e3bc-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e3bc-176">Request</span></span>
<span data-ttu-id="0e3bc-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e3bc-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3bc-178">Response</span></span>
<span data-ttu-id="0e3bc-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e3bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




