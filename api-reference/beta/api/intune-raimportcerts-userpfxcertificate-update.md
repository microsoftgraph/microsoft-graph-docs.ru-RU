---
title: Обновление userPFXCertificate
description: Обновление свойств объекта userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 745faa38ded53e357cf78a56fcf0b4ab1b2298db
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152189"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="7cccb-103">Обновление userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="7cccb-103">Update userPFXCertificate</span></span>

<span data-ttu-id="7cccb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cccb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cccb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cccb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cccb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7cccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cccb-107">Обновление свойств объекта [userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="7cccb-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cccb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7cccb-108">Prerequisites</span></span>
<span data-ttu-id="7cccb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cccb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cccb-111">Permission type</span></span>|<span data-ttu-id="7cccb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cccb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cccb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cccb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cccb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cccb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cccb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cccb-116">Not supported.</span></span>|
|<span data-ttu-id="7cccb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7cccb-117">Application</span></span>|<span data-ttu-id="7cccb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cccb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cccb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="7cccb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7cccb-120">Request headers</span></span>
|<span data-ttu-id="7cccb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cccb-121">Header</span></span>|<span data-ttu-id="7cccb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7cccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cccb-123">Authorization</span></span>|<span data-ttu-id="7cccb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cccb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7cccb-125">Accept</span></span>|<span data-ttu-id="7cccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cccb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cccb-127">Request body</span></span>
<span data-ttu-id="7cccb-128">В теле запроса поставляем представление JSON для [объекта userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="7cccb-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="7cccb-129">В следующей таблице показаны свойства, необходимые при создании [пользователяPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="7cccb-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="7cccb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cccb-130">Property</span></span>|<span data-ttu-id="7cccb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7cccb-131">Type</span></span>|<span data-ttu-id="7cccb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7cccb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cccb-133">id</span><span class="sxs-lookup"><span data-stu-id="7cccb-133">id</span></span>|<span data-ttu-id="7cccb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7cccb-134">String</span></span>|<span data-ttu-id="7cccb-135">Уникальный идентификатор для сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="7cccb-136">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="7cccb-136">thumbprint</span></span>|<span data-ttu-id="7cccb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7cccb-137">String</span></span>|<span data-ttu-id="7cccb-138">Отпечатки sha-1 сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="7cccb-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="7cccb-139">intendedPurpose</span></span>|[<span data-ttu-id="7cccb-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="7cccb-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="7cccb-141">Предназначение сертификата с точки зрения развертывания.</span><span class="sxs-lookup"><span data-stu-id="7cccb-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="7cccb-142">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="7cccb-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="7cccb-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cccb-143">userPrincipalName</span></span>|<span data-ttu-id="7cccb-144">String</span><span class="sxs-lookup"><span data-stu-id="7cccb-144">String</span></span>|<span data-ttu-id="7cccb-145">Имя пользователя сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="7cccb-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7cccb-146">startDateTime</span></span>|<span data-ttu-id="7cccb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cccb-147">DateTimeOffset</span></span>|<span data-ttu-id="7cccb-148">Дата начала действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7cccb-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="7cccb-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7cccb-149">expirationDateTime</span></span>|<span data-ttu-id="7cccb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cccb-150">DateTimeOffset</span></span>|<span data-ttu-id="7cccb-151">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7cccb-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="7cccb-152">providerName</span><span class="sxs-lookup"><span data-stu-id="7cccb-152">providerName</span></span>|<span data-ttu-id="7cccb-153">Строка</span><span class="sxs-lookup"><span data-stu-id="7cccb-153">String</span></span>|<span data-ttu-id="7cccb-154">Поставщик криптографии, используемый для шифрования этого blob.</span><span class="sxs-lookup"><span data-stu-id="7cccb-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="7cccb-155">keyName</span><span class="sxs-lookup"><span data-stu-id="7cccb-155">keyName</span></span>|<span data-ttu-id="7cccb-156">Строка</span><span class="sxs-lookup"><span data-stu-id="7cccb-156">String</span></span>|<span data-ttu-id="7cccb-157">Имя ключа (в пределах поставщика), используемого для шифрования blob.</span><span class="sxs-lookup"><span data-stu-id="7cccb-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="7cccb-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="7cccb-158">paddingScheme</span></span>|[<span data-ttu-id="7cccb-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="7cccb-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="7cccb-160">Схема заполнения, используемая поставщиком при шифровании и расшифровке.</span><span class="sxs-lookup"><span data-stu-id="7cccb-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="7cccb-161">Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="7cccb-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="7cccb-162">зашифрованныйPfxBlob</span><span class="sxs-lookup"><span data-stu-id="7cccb-162">encryptedPfxBlob</span></span>|<span data-ttu-id="7cccb-163">Binary</span><span class="sxs-lookup"><span data-stu-id="7cccb-163">Binary</span></span>|<span data-ttu-id="7cccb-164">Зашифрованный BLOB PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="7cccb-165">зашифрованныйPfxPassword</span><span class="sxs-lookup"><span data-stu-id="7cccb-165">encryptedPfxPassword</span></span>|<span data-ttu-id="7cccb-166">Строка</span><span class="sxs-lookup"><span data-stu-id="7cccb-166">String</span></span>|<span data-ttu-id="7cccb-167">Зашифрованный пароль PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="7cccb-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cccb-168">createdDateTime</span></span>|<span data-ttu-id="7cccb-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cccb-169">DateTimeOffset</span></span>|<span data-ttu-id="7cccb-170">Дата и время импорта этого сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="7cccb-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cccb-171">lastModifiedDateTime</span></span>|<span data-ttu-id="7cccb-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cccb-172">DateTimeOffset</span></span>|<span data-ttu-id="7cccb-173">Дата и время последнего изменения этого сертификата PFX.</span><span class="sxs-lookup"><span data-stu-id="7cccb-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="7cccb-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cccb-174">Response</span></span>
<span data-ttu-id="7cccb-175">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7cccb-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cccb-176">Пример</span><span class="sxs-lookup"><span data-stu-id="7cccb-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cccb-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-177">Request</span></span>
<span data-ttu-id="7cccb-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cccb-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
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

### <a name="response"></a><span data-ttu-id="7cccb-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cccb-179">Response</span></span>
<span data-ttu-id="7cccb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




