---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойств объекта symantecCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56c665a75d594d2f1ad0e28c3800348f0fbde9c3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957530"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="47442-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="47442-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="47442-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47442-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47442-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47442-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47442-106">Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="47442-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47442-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47442-107">Prerequisites</span></span>
<span data-ttu-id="47442-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47442-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47442-110">Permission type</span></span>|<span data-ttu-id="47442-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47442-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47442-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47442-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47442-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47442-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47442-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47442-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47442-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47442-115">Not supported.</span></span>|
|<span data-ttu-id="47442-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47442-116">Application</span></span>|<span data-ttu-id="47442-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47442-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47442-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47442-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="47442-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47442-119">Request headers</span></span>
|<span data-ttu-id="47442-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47442-120">Header</span></span>|<span data-ttu-id="47442-121">Значение</span><span class="sxs-lookup"><span data-stu-id="47442-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47442-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47442-122">Authorization</span></span>|<span data-ttu-id="47442-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47442-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47442-124">Accept</span><span class="sxs-lookup"><span data-stu-id="47442-124">Accept</span></span>|<span data-ttu-id="47442-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47442-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47442-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47442-126">Request body</span></span>
<span data-ttu-id="47442-127">В тексте запроса добавьте представление объекта [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47442-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="47442-128">В следующей таблице приведены свойства, необходимые при создании [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="47442-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="47442-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="47442-129">Property</span></span>|<span data-ttu-id="47442-130">Тип</span><span class="sxs-lookup"><span data-stu-id="47442-130">Type</span></span>|<span data-ttu-id="47442-131">Описание</span><span class="sxs-lookup"><span data-stu-id="47442-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47442-132">id</span><span class="sxs-lookup"><span data-stu-id="47442-132">id</span></span>|<span data-ttu-id="47442-133">String</span><span class="sxs-lookup"><span data-stu-id="47442-133">String</span></span>|<span data-ttu-id="47442-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47442-134">The key of the entity.</span></span>|
|<span data-ttu-id="47442-135">содержимое</span><span class="sxs-lookup"><span data-stu-id="47442-135">content</span></span>|<span data-ttu-id="47442-136">Binary</span><span class="sxs-lookup"><span data-stu-id="47442-136">Binary</span></span>|<span data-ttu-id="47442-137">Сертификат подписи кода Windows Symantec в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="47442-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="47442-138">status</span><span class="sxs-lookup"><span data-stu-id="47442-138">status</span></span>|[<span data-ttu-id="47442-139">Цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="47442-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="47442-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="47442-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="47442-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="47442-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="47442-142">password</span><span class="sxs-lookup"><span data-stu-id="47442-142">password</span></span>|<span data-ttu-id="47442-143">Строка</span><span class="sxs-lookup"><span data-stu-id="47442-143">String</span></span>|<span data-ttu-id="47442-144">Пароль, необходимый для PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="47442-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="47442-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="47442-145">subjectName</span></span>|<span data-ttu-id="47442-146">String</span><span class="sxs-lookup"><span data-stu-id="47442-146">String</span></span>|<span data-ttu-id="47442-147">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="47442-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="47442-148">subject</span><span class="sxs-lookup"><span data-stu-id="47442-148">subject</span></span>|<span data-ttu-id="47442-149">String</span><span class="sxs-lookup"><span data-stu-id="47442-149">String</span></span>|<span data-ttu-id="47442-150">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="47442-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="47442-151">Иссуернаме</span><span class="sxs-lookup"><span data-stu-id="47442-151">issuerName</span></span>|<span data-ttu-id="47442-152">String</span><span class="sxs-lookup"><span data-stu-id="47442-152">String</span></span>|<span data-ttu-id="47442-153">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="47442-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="47442-154">имени</span><span class="sxs-lookup"><span data-stu-id="47442-154">issuer</span></span>|<span data-ttu-id="47442-155">String</span><span class="sxs-lookup"><span data-stu-id="47442-155">String</span></span>|<span data-ttu-id="47442-156">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="47442-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="47442-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="47442-157">expirationDateTime</span></span>|<span data-ttu-id="47442-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47442-158">DateTimeOffset</span></span>|<span data-ttu-id="47442-159">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="47442-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="47442-160">Уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="47442-160">uploadDateTime</span></span>|<span data-ttu-id="47442-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47442-161">DateTimeOffset</span></span>|<span data-ttu-id="47442-162">Тип сертификата соПроектировании в качестве сертификата Symantec.</span><span class="sxs-lookup"><span data-stu-id="47442-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="47442-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="47442-163">Response</span></span>
<span data-ttu-id="47442-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47442-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47442-165">Пример</span><span class="sxs-lookup"><span data-stu-id="47442-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="47442-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="47442-166">Request</span></span>
<span data-ttu-id="47442-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47442-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47442-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="47442-168">Response</span></span>
<span data-ttu-id="47442-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47442-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




