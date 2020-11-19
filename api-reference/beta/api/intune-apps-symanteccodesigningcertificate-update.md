---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойств объекта symantecCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a31fe8fcaaf27e37fc1119460e521ad18339dcee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247687"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="e4ed2-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="e4ed2-103">Update symantecCodeSigningCertificate</span></span>

<span data-ttu-id="e4ed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4ed2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4ed2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ed2-107">Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="e4ed2-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4ed2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4ed2-108">Prerequisites</span></span>
<span data-ttu-id="e4ed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ed2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4ed2-111">Permission type</span></span>|<span data-ttu-id="e4ed2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4ed2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4ed2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4ed2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4ed2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ed2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4ed2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4ed2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4ed2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-116">Not supported.</span></span>|
|<span data-ttu-id="e4ed2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4ed2-117">Application</span></span>|<span data-ttu-id="e4ed2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ed2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4ed2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4ed2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e4ed2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4ed2-120">Request headers</span></span>
|<span data-ttu-id="e4ed2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4ed2-121">Header</span></span>|<span data-ttu-id="e4ed2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4ed2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4ed2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4ed2-123">Authorization</span></span>|<span data-ttu-id="e4ed2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4ed2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4ed2-125">Accept</span></span>|<span data-ttu-id="e4ed2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4ed2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4ed2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4ed2-127">Request body</span></span>
<span data-ttu-id="e4ed2-128">В тексте запроса добавьте представление объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="e4ed2-129">В следующей таблице приведены свойства, необходимые при создании [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e4ed2-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="e4ed2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4ed2-130">Property</span></span>|<span data-ttu-id="e4ed2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4ed2-131">Type</span></span>|<span data-ttu-id="e4ed2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ed2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ed2-133">id</span><span class="sxs-lookup"><span data-stu-id="e4ed2-133">id</span></span>|<span data-ttu-id="e4ed2-134">String</span><span class="sxs-lookup"><span data-stu-id="e4ed2-134">String</span></span>|<span data-ttu-id="e4ed2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-135">The key of the entity.</span></span>|
|<span data-ttu-id="e4ed2-136">содержимое</span><span class="sxs-lookup"><span data-stu-id="e4ed2-136">content</span></span>|<span data-ttu-id="e4ed2-137">Binary</span><span class="sxs-lookup"><span data-stu-id="e4ed2-137">Binary</span></span>|<span data-ttu-id="e4ed2-138">Сертификат Code-Signing Windows Symantec в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="e4ed2-139">status</span><span class="sxs-lookup"><span data-stu-id="e4ed2-139">status</span></span>|[<span data-ttu-id="e4ed2-140">цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="e4ed2-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="e4ed2-141">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="e4ed2-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="e4ed2-143">password</span><span class="sxs-lookup"><span data-stu-id="e4ed2-143">password</span></span>|<span data-ttu-id="e4ed2-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ed2-144">String</span></span>|<span data-ttu-id="e4ed2-145">Пароль, необходимый для PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="e4ed2-146">subjectName</span><span class="sxs-lookup"><span data-stu-id="e4ed2-146">subjectName</span></span>|<span data-ttu-id="e4ed2-147">String</span><span class="sxs-lookup"><span data-stu-id="e4ed2-147">String</span></span>|<span data-ttu-id="e4ed2-148">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="e4ed2-149">subject</span><span class="sxs-lookup"><span data-stu-id="e4ed2-149">subject</span></span>|<span data-ttu-id="e4ed2-150">String</span><span class="sxs-lookup"><span data-stu-id="e4ed2-150">String</span></span>|<span data-ttu-id="e4ed2-151">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="e4ed2-152">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="e4ed2-152">issuerName</span></span>|<span data-ttu-id="e4ed2-153">String</span><span class="sxs-lookup"><span data-stu-id="e4ed2-153">String</span></span>|<span data-ttu-id="e4ed2-154">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="e4ed2-155">имени</span><span class="sxs-lookup"><span data-stu-id="e4ed2-155">issuer</span></span>|<span data-ttu-id="e4ed2-156">String</span><span class="sxs-lookup"><span data-stu-id="e4ed2-156">String</span></span>|<span data-ttu-id="e4ed2-157">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="e4ed2-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ed2-158">expirationDateTime</span></span>|<span data-ttu-id="e4ed2-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ed2-159">DateTimeOffset</span></span>|<span data-ttu-id="e4ed2-160">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="e4ed2-161">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="e4ed2-161">uploadDateTime</span></span>|<span data-ttu-id="e4ed2-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ed2-162">DateTimeOffset</span></span>|<span data-ttu-id="e4ed2-163">Тип сертификата сопроектировании в качестве сертификата Symantec.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="e4ed2-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ed2-164">Response</span></span>
<span data-ttu-id="e4ed2-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4ed2-166">Пример</span><span class="sxs-lookup"><span data-stu-id="e4ed2-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4ed2-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4ed2-167">Request</span></span>
<span data-ttu-id="e4ed2-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4ed2-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ed2-169">Response</span></span>
<span data-ttu-id="e4ed2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4ed2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




