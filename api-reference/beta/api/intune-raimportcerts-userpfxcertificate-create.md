---
title: Создание Усерпфксцертификате
description: Создание нового объекта Усерпфксцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f7fb02f0081e68de15b11f751d9c339871e2209
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993797"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="9d6a0-103">Создание Усерпфксцертификате</span><span class="sxs-lookup"><span data-stu-id="9d6a0-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="9d6a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d6a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d6a0-106">Создание нового объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="9d6a0-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d6a0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d6a0-107">Prerequisites</span></span>
<span data-ttu-id="9d6a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d6a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d6a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d6a0-110">Permission type</span></span>|<span data-ttu-id="9d6a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d6a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d6a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d6a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d6a0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d6a0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d6a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d6a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d6a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-115">Not supported.</span></span>|
|<span data-ttu-id="9d6a0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d6a0-116">Application</span></span>|<span data-ttu-id="9d6a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d6a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d6a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="9d6a0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d6a0-119">Request headers</span></span>
|<span data-ttu-id="9d6a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d6a0-120">Header</span></span>|<span data-ttu-id="9d6a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9d6a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d6a0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d6a0-122">Authorization</span></span>|<span data-ttu-id="9d6a0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d6a0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9d6a0-124">Accept</span></span>|<span data-ttu-id="9d6a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d6a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6a0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d6a0-126">Request body</span></span>
<span data-ttu-id="9d6a0-127">В тексте запроса добавьте представление объекта Усерпфксцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="9d6a0-128">В следующей таблице приведены свойства, необходимые при создании Усерпфксцертификате.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="9d6a0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d6a0-129">Property</span></span>|<span data-ttu-id="9d6a0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9d6a0-130">Type</span></span>|<span data-ttu-id="9d6a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9d6a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6a0-132">id</span><span class="sxs-lookup"><span data-stu-id="9d6a0-132">id</span></span>|<span data-ttu-id="9d6a0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9d6a0-133">String</span></span>|<span data-ttu-id="9d6a0-134">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="9d6a0-135">отпечаток</span><span class="sxs-lookup"><span data-stu-id="9d6a0-135">thumbprint</span></span>|<span data-ttu-id="9d6a0-136">String</span><span class="sxs-lookup"><span data-stu-id="9d6a0-136">String</span></span>|<span data-ttu-id="9d6a0-137">Отпечаток SHA-1 сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="9d6a0-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9d6a0-138">intendedPurpose</span></span>|[<span data-ttu-id="9d6a0-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9d6a0-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="9d6a0-140">Сертификат, предназначенный для целей из точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="9d6a0-141">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="9d6a0-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d6a0-142">userPrincipalName</span></span>|<span data-ttu-id="9d6a0-143">String</span><span class="sxs-lookup"><span data-stu-id="9d6a0-143">String</span></span>|<span data-ttu-id="9d6a0-144">Имя участника-пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="9d6a0-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6a0-145">startDateTime</span></span>|<span data-ttu-id="9d6a0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6a0-146">DateTimeOffset</span></span>|<span data-ttu-id="9d6a0-147">Дата и время начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="9d6a0-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6a0-148">expirationDateTime</span></span>|<span data-ttu-id="9d6a0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6a0-149">DateTimeOffset</span></span>|<span data-ttu-id="9d6a0-150">Дата и время действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="9d6a0-151">providerName</span><span class="sxs-lookup"><span data-stu-id="9d6a0-151">providerName</span></span>|<span data-ttu-id="9d6a0-152">String</span><span class="sxs-lookup"><span data-stu-id="9d6a0-152">String</span></span>|<span data-ttu-id="9d6a0-153">Поставщик криптографии, используемый для шифрования этого объекта BLOB.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="9d6a0-154">keyName</span><span class="sxs-lookup"><span data-stu-id="9d6a0-154">keyName</span></span>|<span data-ttu-id="9d6a0-155">String</span><span class="sxs-lookup"><span data-stu-id="9d6a0-155">String</span></span>|<span data-ttu-id="9d6a0-156">Имя ключа (в пределах поставщика), используемого для шифрования большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="9d6a0-157">Паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="9d6a0-157">paddingScheme</span></span>|[<span data-ttu-id="9d6a0-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="9d6a0-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="9d6a0-159">Схема заполнения, используемая поставщиком во время шифрования и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="9d6a0-160">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="9d6a0-161">Енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="9d6a0-161">encryptedPfxBlob</span></span>|<span data-ttu-id="9d6a0-162">Binary</span><span class="sxs-lookup"><span data-stu-id="9d6a0-162">Binary</span></span>|<span data-ttu-id="9d6a0-163">Зашифрованный BLOB-объект PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="9d6a0-164">Енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="9d6a0-164">encryptedPfxPassword</span></span>|<span data-ttu-id="9d6a0-165">String</span><span class="sxs-lookup"><span data-stu-id="9d6a0-165">String</span></span>|<span data-ttu-id="9d6a0-166">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="9d6a0-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6a0-167">createdDateTime</span></span>|<span data-ttu-id="9d6a0-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6a0-168">DateTimeOffset</span></span>|<span data-ttu-id="9d6a0-169">Дата и время импорта этого PFX-сертификата.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="9d6a0-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6a0-170">lastModifiedDateTime</span></span>|<span data-ttu-id="9d6a0-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6a0-171">DateTimeOffset</span></span>|<span data-ttu-id="9d6a0-172">Дата и время последнего изменения сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9d6a0-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d6a0-173">Response</span></span>
<span data-ttu-id="9d6a0-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d6a0-175">Пример</span><span class="sxs-lookup"><span data-stu-id="9d6a0-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d6a0-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d6a0-176">Request</span></span>
<span data-ttu-id="9d6a0-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d6a0-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d6a0-178">Response</span></span>
<span data-ttu-id="9d6a0-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d6a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





