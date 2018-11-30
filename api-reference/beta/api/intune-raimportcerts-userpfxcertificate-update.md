---
title: Обновление userPFXCertificate
description: Обновление свойства объекта userPFXCertificate.
ms.openlocfilehash: 9fde1e8ff073df7acf76119ace0848616424951a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074595"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="3b74e-103">Обновление userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="3b74e-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="3b74e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b74e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b74e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b74e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b74e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b74e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b74e-107">Обновление свойства объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b74e-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b74e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b74e-108">Prerequisites</span></span>
<span data-ttu-id="3b74e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b74e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b74e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b74e-111">Permission type</span></span>|<span data-ttu-id="3b74e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b74e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b74e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b74e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b74e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b74e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b74e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b74e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b74e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b74e-116">Not supported.</span></span>|
|<span data-ttu-id="3b74e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b74e-117">Application</span></span>|<span data-ttu-id="3b74e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b74e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b74e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b74e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="3b74e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b74e-120">Request headers</span></span>
|<span data-ttu-id="3b74e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b74e-121">Header</span></span>|<span data-ttu-id="3b74e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b74e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b74e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b74e-123">Authorization</span></span>|<span data-ttu-id="3b74e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b74e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b74e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b74e-125">Accept</span></span>|<span data-ttu-id="3b74e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b74e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b74e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b74e-127">Request body</span></span>
<span data-ttu-id="3b74e-128">В тексте запроса укажите представление JSON для объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b74e-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="3b74e-129">В следующей таблице показаны свойства, которые необходимы для создания [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3b74e-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="3b74e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b74e-130">Property</span></span>|<span data-ttu-id="3b74e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b74e-131">Type</span></span>|<span data-ttu-id="3b74e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b74e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b74e-133">id</span><span class="sxs-lookup"><span data-stu-id="3b74e-133">id</span></span>|<span data-ttu-id="3b74e-134">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-134">String</span></span>|<span data-ttu-id="3b74e-135">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="3b74e-136">отпечаток</span><span class="sxs-lookup"><span data-stu-id="3b74e-136">thumbprint</span></span>|<span data-ttu-id="3b74e-137">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-137">String</span></span>|<span data-ttu-id="3b74e-138">Отпечаток сертификата, PFX SHA-1.</span><span class="sxs-lookup"><span data-stu-id="3b74e-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="3b74e-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3b74e-139">intendedPurpose</span></span>|[<span data-ttu-id="3b74e-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3b74e-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="3b74e-141">Сертификата своей целью с точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="3b74e-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="3b74e-142">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="3b74e-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="3b74e-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b74e-143">userPrincipalName</span></span>|<span data-ttu-id="3b74e-144">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-144">String</span></span>|<span data-ttu-id="3b74e-145">Имя участника-пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="3b74e-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b74e-146">startDateTime</span></span>|<span data-ttu-id="3b74e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b74e-147">DateTimeOffset</span></span>|<span data-ttu-id="3b74e-148">Дата и время начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3b74e-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="3b74e-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b74e-149">expirationDateTime</span></span>|<span data-ttu-id="3b74e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b74e-150">DateTimeOffset</span></span>|<span data-ttu-id="3b74e-151">Его допустимость Дата и время окончания.</span><span class="sxs-lookup"><span data-stu-id="3b74e-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="3b74e-152">providerName</span><span class="sxs-lookup"><span data-stu-id="3b74e-152">providerName</span></span>|<span data-ttu-id="3b74e-153">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-153">String</span></span>|<span data-ttu-id="3b74e-154">Поставщик криптографии для шифрования в этом больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="3b74e-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="3b74e-155">keyName</span><span class="sxs-lookup"><span data-stu-id="3b74e-155">keyName</span></span>|<span data-ttu-id="3b74e-156">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-156">String</span></span>|<span data-ttu-id="3b74e-157">Имя ключа (в рамках поставщика) используется для шифрования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="3b74e-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="3b74e-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="3b74e-158">paddingScheme</span></span>|[<span data-ttu-id="3b74e-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="3b74e-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="3b74e-160">Заполнение схемы, используемый поставщиком во время шифрования и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="3b74e-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="3b74e-161">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="3b74e-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="3b74e-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="3b74e-162">encryptedPfxBlob</span></span>|<span data-ttu-id="3b74e-163">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3b74e-163">Binary</span></span>|<span data-ttu-id="3b74e-164">Зашифрованные больших двоичных объектов PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="3b74e-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="3b74e-165">encryptedPfxPassword</span></span>|<span data-ttu-id="3b74e-166">String</span><span class="sxs-lookup"><span data-stu-id="3b74e-166">String</span></span>|<span data-ttu-id="3b74e-167">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="3b74e-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b74e-168">createdDateTime</span></span>|<span data-ttu-id="3b74e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b74e-169">DateTimeOffset</span></span>|<span data-ttu-id="3b74e-170">Дата и время при импорте сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="3b74e-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b74e-171">lastModifiedDateTime</span></span>|<span data-ttu-id="3b74e-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b74e-172">DateTimeOffset</span></span>|<span data-ttu-id="3b74e-173">Дата и время последнего изменения этого сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="3b74e-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3b74e-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b74e-174">Response</span></span>
<span data-ttu-id="3b74e-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b74e-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b74e-176">Пример</span><span class="sxs-lookup"><span data-stu-id="3b74e-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b74e-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b74e-177">Request</span></span>
<span data-ttu-id="3b74e-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b74e-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 530

{
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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3b74e-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b74e-179">Response</span></span>
<span data-ttu-id="3b74e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3b74e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





