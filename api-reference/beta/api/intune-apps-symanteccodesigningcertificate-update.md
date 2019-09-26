---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойств объекта symantecCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14bf754dbb98d631ac24c6a548c57650268c9d11
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172270"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="44efc-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="44efc-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="44efc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44efc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44efc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44efc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44efc-106">Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="44efc-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44efc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44efc-107">Prerequisites</span></span>
<span data-ttu-id="44efc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44efc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44efc-110">Permission type</span></span>|<span data-ttu-id="44efc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44efc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44efc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44efc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44efc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44efc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44efc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44efc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44efc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44efc-115">Not supported.</span></span>|
|<span data-ttu-id="44efc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44efc-116">Application</span></span>|<span data-ttu-id="44efc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44efc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44efc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44efc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="44efc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44efc-119">Request headers</span></span>
|<span data-ttu-id="44efc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44efc-120">Header</span></span>|<span data-ttu-id="44efc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44efc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44efc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44efc-122">Authorization</span></span>|<span data-ttu-id="44efc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44efc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44efc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44efc-124">Accept</span></span>|<span data-ttu-id="44efc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44efc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44efc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44efc-126">Request body</span></span>
<span data-ttu-id="44efc-127">В тексте запроса добавьте представление объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44efc-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="44efc-128">В следующей таблице приведены свойства, необходимые при создании [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="44efc-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="44efc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44efc-129">Property</span></span>|<span data-ttu-id="44efc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44efc-130">Type</span></span>|<span data-ttu-id="44efc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44efc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44efc-132">id</span><span class="sxs-lookup"><span data-stu-id="44efc-132">id</span></span>|<span data-ttu-id="44efc-133">String</span><span class="sxs-lookup"><span data-stu-id="44efc-133">String</span></span>|<span data-ttu-id="44efc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44efc-134">The key of the entity.</span></span>|
|<span data-ttu-id="44efc-135">содержимое</span><span class="sxs-lookup"><span data-stu-id="44efc-135">content</span></span>|<span data-ttu-id="44efc-136">Binary</span><span class="sxs-lookup"><span data-stu-id="44efc-136">Binary</span></span>|<span data-ttu-id="44efc-137">Сертификат подписи кода Windows Symantec в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="44efc-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="44efc-138">status</span><span class="sxs-lookup"><span data-stu-id="44efc-138">status</span></span>|[<span data-ttu-id="44efc-139">цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="44efc-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="44efc-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="44efc-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="44efc-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="44efc-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="44efc-142">password</span><span class="sxs-lookup"><span data-stu-id="44efc-142">password</span></span>|<span data-ttu-id="44efc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="44efc-143">String</span></span>|<span data-ttu-id="44efc-144">Пароль, необходимый для PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="44efc-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="44efc-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="44efc-145">subjectName</span></span>|<span data-ttu-id="44efc-146">String</span><span class="sxs-lookup"><span data-stu-id="44efc-146">String</span></span>|<span data-ttu-id="44efc-147">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="44efc-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="44efc-148">subject</span><span class="sxs-lookup"><span data-stu-id="44efc-148">subject</span></span>|<span data-ttu-id="44efc-149">String</span><span class="sxs-lookup"><span data-stu-id="44efc-149">String</span></span>|<span data-ttu-id="44efc-150">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="44efc-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="44efc-151">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="44efc-151">issuerName</span></span>|<span data-ttu-id="44efc-152">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-152">String</span></span>|<span data-ttu-id="44efc-153">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="44efc-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="44efc-154">имени</span><span class="sxs-lookup"><span data-stu-id="44efc-154">issuer</span></span>|<span data-ttu-id="44efc-155">String.</span><span class="sxs-lookup"><span data-stu-id="44efc-155">String</span></span>|<span data-ttu-id="44efc-156">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="44efc-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="44efc-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="44efc-157">expirationDateTime</span></span>|<span data-ttu-id="44efc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44efc-158">DateTimeOffset</span></span>|<span data-ttu-id="44efc-159">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="44efc-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="44efc-160">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="44efc-160">uploadDateTime</span></span>|<span data-ttu-id="44efc-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44efc-161">DateTimeOffset</span></span>|<span data-ttu-id="44efc-162">Тип сертификата сопроектировании в качестве сертификата Symantec.</span><span class="sxs-lookup"><span data-stu-id="44efc-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="44efc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="44efc-163">Response</span></span>
<span data-ttu-id="44efc-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44efc-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44efc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="44efc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="44efc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="44efc-166">Request</span></span>
<span data-ttu-id="44efc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44efc-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="44efc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="44efc-168">Response</span></span>
<span data-ttu-id="44efc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44efc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```




