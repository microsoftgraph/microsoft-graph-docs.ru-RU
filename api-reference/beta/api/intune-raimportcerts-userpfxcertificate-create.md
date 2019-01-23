---
title: Создание userPFXCertificate
description: Создание нового объекта userPFXCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8896e3bb300507f0d1a89892852a2e1d4865d9b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418171"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="42191-103">Создание userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="42191-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="42191-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42191-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42191-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42191-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42191-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42191-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42191-107">Создание нового объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="42191-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42191-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="42191-108">Prerequisites</span></span>
<span data-ttu-id="42191-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42191-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42191-111">Permission type</span></span>|<span data-ttu-id="42191-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42191-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42191-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42191-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42191-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42191-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42191-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42191-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42191-116">Not supported.</span></span>|
|<span data-ttu-id="42191-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42191-117">Application</span></span>|<span data-ttu-id="42191-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42191-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42191-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42191-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="42191-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42191-120">Request headers</span></span>
|<span data-ttu-id="42191-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42191-121">Header</span></span>|<span data-ttu-id="42191-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42191-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42191-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42191-123">Authorization</span></span>|<span data-ttu-id="42191-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42191-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42191-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42191-125">Accept</span></span>|<span data-ttu-id="42191-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42191-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42191-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42191-127">Request body</span></span>
<span data-ttu-id="42191-128">В тексте запроса укажите представление JSON для объекта userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="42191-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="42191-129">В следующей таблице показаны свойства, которые необходимы для создания userPFXCertificate.</span><span class="sxs-lookup"><span data-stu-id="42191-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="42191-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42191-130">Property</span></span>|<span data-ttu-id="42191-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42191-131">Type</span></span>|<span data-ttu-id="42191-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42191-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42191-133">id</span><span class="sxs-lookup"><span data-stu-id="42191-133">id</span></span>|<span data-ttu-id="42191-134">String</span><span class="sxs-lookup"><span data-stu-id="42191-134">String</span></span>|<span data-ttu-id="42191-135">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="42191-136">отпечаток</span><span class="sxs-lookup"><span data-stu-id="42191-136">thumbprint</span></span>|<span data-ttu-id="42191-137">String</span><span class="sxs-lookup"><span data-stu-id="42191-137">String</span></span>|<span data-ttu-id="42191-138">Отпечаток сертификата, PFX SHA-1.</span><span class="sxs-lookup"><span data-stu-id="42191-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="42191-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="42191-139">intendedPurpose</span></span>|[<span data-ttu-id="42191-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="42191-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="42191-141">Сертификата своей целью с точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="42191-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="42191-142">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="42191-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="42191-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42191-143">userPrincipalName</span></span>|<span data-ttu-id="42191-144">String</span><span class="sxs-lookup"><span data-stu-id="42191-144">String</span></span>|<span data-ttu-id="42191-145">Имя участника-пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="42191-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="42191-146">startDateTime</span></span>|<span data-ttu-id="42191-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42191-147">DateTimeOffset</span></span>|<span data-ttu-id="42191-148">Дата и время начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="42191-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="42191-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="42191-149">expirationDateTime</span></span>|<span data-ttu-id="42191-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42191-150">DateTimeOffset</span></span>|<span data-ttu-id="42191-151">Его допустимость Дата и время окончания.</span><span class="sxs-lookup"><span data-stu-id="42191-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="42191-152">providerName</span><span class="sxs-lookup"><span data-stu-id="42191-152">providerName</span></span>|<span data-ttu-id="42191-153">String</span><span class="sxs-lookup"><span data-stu-id="42191-153">String</span></span>|<span data-ttu-id="42191-154">Поставщик криптографии для шифрования в этом больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="42191-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="42191-155">keyName</span><span class="sxs-lookup"><span data-stu-id="42191-155">keyName</span></span>|<span data-ttu-id="42191-156">String</span><span class="sxs-lookup"><span data-stu-id="42191-156">String</span></span>|<span data-ttu-id="42191-157">Имя ключа (в рамках поставщика) используется для шифрования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="42191-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="42191-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="42191-158">paddingScheme</span></span>|[<span data-ttu-id="42191-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="42191-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="42191-160">Заполнение схемы, используемый поставщиком во время шифрования и расшифровки.</span><span class="sxs-lookup"><span data-stu-id="42191-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="42191-161">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="42191-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="42191-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="42191-162">encryptedPfxBlob</span></span>|<span data-ttu-id="42191-163">Binary</span><span class="sxs-lookup"><span data-stu-id="42191-163">Binary</span></span>|<span data-ttu-id="42191-164">Зашифрованные больших двоичных объектов PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="42191-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="42191-165">encryptedPfxPassword</span></span>|<span data-ttu-id="42191-166">String</span><span class="sxs-lookup"><span data-stu-id="42191-166">String</span></span>|<span data-ttu-id="42191-167">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="42191-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42191-168">createdDateTime</span></span>|<span data-ttu-id="42191-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42191-169">DateTimeOffset</span></span>|<span data-ttu-id="42191-170">Дата и время при импорте сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="42191-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42191-171">lastModifiedDateTime</span></span>|<span data-ttu-id="42191-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42191-172">DateTimeOffset</span></span>|<span data-ttu-id="42191-173">Дата и время последнего изменения этого сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="42191-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="42191-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="42191-174">Response</span></span>
<span data-ttu-id="42191-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42191-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42191-176">Пример</span><span class="sxs-lookup"><span data-stu-id="42191-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="42191-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="42191-177">Request</span></span>
<span data-ttu-id="42191-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42191-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42191-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="42191-179">Response</span></span>
<span data-ttu-id="42191-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42191-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




