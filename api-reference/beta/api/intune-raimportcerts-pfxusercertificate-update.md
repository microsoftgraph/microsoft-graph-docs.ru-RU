---
title: Обновление Пфксусерцертификате
description: Обновление свойств объекта Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6756a6c35818426790e24d7f348ca760355ffec6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726149"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="6ebff-103">Обновление Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="6ebff-103">Update pfxUserCertificate</span></span>

> <span data-ttu-id="6ebff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ebff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ebff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ebff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ebff-106">Обновление свойств объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="6ebff-106">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ebff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ebff-107">Prerequisites</span></span>
<span data-ttu-id="6ebff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ebff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ebff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ebff-110">Permission type</span></span>|<span data-ttu-id="6ebff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ebff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ebff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ebff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ebff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ebff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ebff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ebff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ebff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ebff-115">Not supported.</span></span>|
|<span data-ttu-id="6ebff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ebff-116">Application</span></span>|<span data-ttu-id="6ebff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ebff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ebff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ebff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="6ebff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ebff-119">Request headers</span></span>
|<span data-ttu-id="6ebff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ebff-120">Header</span></span>|<span data-ttu-id="6ebff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ebff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ebff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ebff-122">Authorization</span></span>|<span data-ttu-id="6ebff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ebff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ebff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ebff-124">Accept</span></span>|<span data-ttu-id="6ebff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ebff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ebff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ebff-126">Request body</span></span>
<span data-ttu-id="6ebff-127">В тексте запроса добавьте представление объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ebff-127">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="6ebff-128">В следующей таблице приведены свойства, необходимые при создании [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="6ebff-128">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="6ebff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ebff-129">Property</span></span>|<span data-ttu-id="6ebff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6ebff-130">Type</span></span>|<span data-ttu-id="6ebff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6ebff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ebff-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="6ebff-132">tenantId</span></span>|<span data-ttu-id="6ebff-133">GUID</span><span class="sxs-lookup"><span data-stu-id="6ebff-133">Guid</span></span>|<span data-ttu-id="6ebff-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-134">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-135">userId</span><span class="sxs-lookup"><span data-stu-id="6ebff-135">userId</span></span>|<span data-ttu-id="6ebff-136">GUID</span><span class="sxs-lookup"><span data-stu-id="6ebff-136">Guid</span></span>|<span data-ttu-id="6ebff-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-137">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-138">отпечаток</span><span class="sxs-lookup"><span data-stu-id="6ebff-138">thumbprint</span></span>|<span data-ttu-id="6ebff-139">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-139">String</span></span>|<span data-ttu-id="6ebff-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-140">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-141">Усерупн</span><span class="sxs-lookup"><span data-stu-id="6ebff-141">userUpn</span></span>|<span data-ttu-id="6ebff-142">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-142">String</span></span>|<span data-ttu-id="6ebff-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-143">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-144">Енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="6ebff-144">encryptedPfxBlob</span></span>|<span data-ttu-id="6ebff-145">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-145">String</span></span>|<span data-ttu-id="6ebff-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-146">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-147">Енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="6ebff-147">encryptedPfxPassword</span></span>|<span data-ttu-id="6ebff-148">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-148">String</span></span>|<span data-ttu-id="6ebff-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-149">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-150">Цертстартдате</span><span class="sxs-lookup"><span data-stu-id="6ebff-150">certStartDate</span></span>|<span data-ttu-id="6ebff-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ebff-151">DateTimeOffset</span></span>|<span data-ttu-id="6ebff-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-152">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-153">Цертекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="6ebff-153">certExpirationDate</span></span>|<span data-ttu-id="6ebff-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ebff-154">DateTimeOffset</span></span>|<span data-ttu-id="6ebff-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-155">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-156">providerName</span><span class="sxs-lookup"><span data-stu-id="6ebff-156">providerName</span></span>|<span data-ttu-id="6ebff-157">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-157">String</span></span>|<span data-ttu-id="6ebff-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-158">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-159">Енкриптионкэйнаме</span><span class="sxs-lookup"><span data-stu-id="6ebff-159">encryptionKeyName</span></span>|<span data-ttu-id="6ebff-160">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-160">String</span></span>|<span data-ttu-id="6ebff-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-161">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-162">Паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="6ebff-162">paddingScheme</span></span>|<span data-ttu-id="6ebff-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6ebff-163">Int32</span></span>|<span data-ttu-id="6ebff-164">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="6ebff-164">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-165">status</span><span class="sxs-lookup"><span data-stu-id="6ebff-165">status</span></span>|<span data-ttu-id="6ebff-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6ebff-166">Int32</span></span>|<span data-ttu-id="6ebff-167">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="6ebff-167">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6ebff-168">intendedPurpose</span></span>|<span data-ttu-id="6ebff-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6ebff-169">Int32</span></span>|<span data-ttu-id="6ebff-170">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="6ebff-170">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="6ebff-171">createdTime</span></span>|<span data-ttu-id="6ebff-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ebff-172">DateTimeOffset</span></span>|<span data-ttu-id="6ebff-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-173">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6ebff-174">isDeleted</span></span>|<span data-ttu-id="6ebff-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ebff-175">Boolean</span></span>|<span data-ttu-id="6ebff-176">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="6ebff-176">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6ebff-177">lastModifiedTime</span></span>|<span data-ttu-id="6ebff-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ebff-178">DateTimeOffset</span></span>|<span data-ttu-id="6ebff-179">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-179">Not yet documented</span></span>|
|<span data-ttu-id="6ebff-180">eTag</span><span class="sxs-lookup"><span data-stu-id="6ebff-180">eTag</span></span>|<span data-ttu-id="6ebff-181">String</span><span class="sxs-lookup"><span data-stu-id="6ebff-181">String</span></span>|<span data-ttu-id="6ebff-182">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6ebff-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6ebff-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ebff-183">Response</span></span>
<span data-ttu-id="6ebff-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ebff-184">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ebff-185">Пример</span><span class="sxs-lookup"><span data-stu-id="6ebff-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ebff-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ebff-186">Request</span></span>
<span data-ttu-id="6ebff-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ebff-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="6ebff-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ebff-188">Response</span></span>
<span data-ttu-id="6ebff-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ebff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```





