---
title: Создание Пфксусерцертификате
description: Создание нового объекта Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bda1a3e6b5f2296b3b7b1da62335cfdf7a8d10aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726150"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="4efb0-103">Создание Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="4efb0-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="4efb0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4efb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4efb0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4efb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4efb0-106">Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="4efb0-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4efb0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4efb0-107">Prerequisites</span></span>
<span data-ttu-id="4efb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4efb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4efb0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4efb0-110">Permission type</span></span>|<span data-ttu-id="4efb0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4efb0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4efb0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4efb0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4efb0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efb0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4efb0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4efb0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4efb0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4efb0-115">Not supported.</span></span>|
|<span data-ttu-id="4efb0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4efb0-116">Application</span></span>|<span data-ttu-id="4efb0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4efb0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4efb0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4efb0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="4efb0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4efb0-119">Request headers</span></span>
|<span data-ttu-id="4efb0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4efb0-120">Header</span></span>|<span data-ttu-id="4efb0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4efb0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4efb0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4efb0-122">Authorization</span></span>|<span data-ttu-id="4efb0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4efb0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4efb0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4efb0-124">Accept</span></span>|<span data-ttu-id="4efb0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4efb0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4efb0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4efb0-126">Request body</span></span>
<span data-ttu-id="4efb0-127">В тексте запроса добавьте представление объекта Пфксусерцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4efb0-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="4efb0-128">В следующей таблице приведены свойства, необходимые при создании Пфксусерцертификате.</span><span class="sxs-lookup"><span data-stu-id="4efb0-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="4efb0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4efb0-129">Property</span></span>|<span data-ttu-id="4efb0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4efb0-130">Type</span></span>|<span data-ttu-id="4efb0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4efb0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4efb0-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="4efb0-132">tenantId</span></span>|<span data-ttu-id="4efb0-133">GUID</span><span class="sxs-lookup"><span data-stu-id="4efb0-133">Guid</span></span>|<span data-ttu-id="4efb0-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-134">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-135">userId</span><span class="sxs-lookup"><span data-stu-id="4efb0-135">userId</span></span>|<span data-ttu-id="4efb0-136">GUID</span><span class="sxs-lookup"><span data-stu-id="4efb0-136">Guid</span></span>|<span data-ttu-id="4efb0-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-137">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-138">отпечаток</span><span class="sxs-lookup"><span data-stu-id="4efb0-138">thumbprint</span></span>|<span data-ttu-id="4efb0-139">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-139">String</span></span>|<span data-ttu-id="4efb0-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-140">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-141">Усерупн</span><span class="sxs-lookup"><span data-stu-id="4efb0-141">userUpn</span></span>|<span data-ttu-id="4efb0-142">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-142">String</span></span>|<span data-ttu-id="4efb0-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-143">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-144">Енкриптедпфксблоб</span><span class="sxs-lookup"><span data-stu-id="4efb0-144">encryptedPfxBlob</span></span>|<span data-ttu-id="4efb0-145">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-145">String</span></span>|<span data-ttu-id="4efb0-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-146">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-147">Енкриптедпфкспассворд</span><span class="sxs-lookup"><span data-stu-id="4efb0-147">encryptedPfxPassword</span></span>|<span data-ttu-id="4efb0-148">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-148">String</span></span>|<span data-ttu-id="4efb0-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-149">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-150">Цертстартдате</span><span class="sxs-lookup"><span data-stu-id="4efb0-150">certStartDate</span></span>|<span data-ttu-id="4efb0-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb0-151">DateTimeOffset</span></span>|<span data-ttu-id="4efb0-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-152">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-153">Цертекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="4efb0-153">certExpirationDate</span></span>|<span data-ttu-id="4efb0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb0-154">DateTimeOffset</span></span>|<span data-ttu-id="4efb0-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-155">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-156">providerName</span><span class="sxs-lookup"><span data-stu-id="4efb0-156">providerName</span></span>|<span data-ttu-id="4efb0-157">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-157">String</span></span>|<span data-ttu-id="4efb0-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-158">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-159">Енкриптионкэйнаме</span><span class="sxs-lookup"><span data-stu-id="4efb0-159">encryptionKeyName</span></span>|<span data-ttu-id="4efb0-160">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-160">String</span></span>|<span data-ttu-id="4efb0-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-161">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-162">Паддингсчеме</span><span class="sxs-lookup"><span data-stu-id="4efb0-162">paddingScheme</span></span>|<span data-ttu-id="4efb0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb0-163">Int32</span></span>|<span data-ttu-id="4efb0-164">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="4efb0-164">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-165">status</span><span class="sxs-lookup"><span data-stu-id="4efb0-165">status</span></span>|<span data-ttu-id="4efb0-166">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb0-166">Int32</span></span>|<span data-ttu-id="4efb0-167">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="4efb0-167">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="4efb0-168">intendedPurpose</span></span>|<span data-ttu-id="4efb0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb0-169">Int32</span></span>|<span data-ttu-id="4efb0-170">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="4efb0-170">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="4efb0-171">createdTime</span></span>|<span data-ttu-id="4efb0-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb0-172">DateTimeOffset</span></span>|<span data-ttu-id="4efb0-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-173">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4efb0-174">isDeleted</span></span>|<span data-ttu-id="4efb0-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4efb0-175">Boolean</span></span>|<span data-ttu-id="4efb0-176">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="4efb0-176">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="4efb0-177">lastModifiedTime</span></span>|<span data-ttu-id="4efb0-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb0-178">DateTimeOffset</span></span>|<span data-ttu-id="4efb0-179">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-179">Not yet documented</span></span>|
|<span data-ttu-id="4efb0-180">eTag</span><span class="sxs-lookup"><span data-stu-id="4efb0-180">eTag</span></span>|<span data-ttu-id="4efb0-181">String</span><span class="sxs-lookup"><span data-stu-id="4efb0-181">String</span></span>|<span data-ttu-id="4efb0-182">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4efb0-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4efb0-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="4efb0-183">Response</span></span>
<span data-ttu-id="4efb0-184">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4efb0-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4efb0-185">Пример</span><span class="sxs-lookup"><span data-stu-id="4efb0-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="4efb0-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="4efb0-186">Request</span></span>
<span data-ttu-id="4efb0-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4efb0-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
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

### <a name="response"></a><span data-ttu-id="4efb0-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="4efb0-188">Response</span></span>
<span data-ttu-id="4efb0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4efb0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





