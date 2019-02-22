---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойств объекта symantecCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a56296956c3955808a308989a0ca8ded5d4ae5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168756"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="8f991-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="8f991-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="8f991-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f991-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f991-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f991-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f991-106">Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="8f991-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f991-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f991-107">Prerequisites</span></span>
<span data-ttu-id="8f991-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f991-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f991-110">Permission type</span></span>|<span data-ttu-id="8f991-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f991-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f991-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f991-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f991-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f991-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f991-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f991-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f991-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f991-115">Not supported.</span></span>|
|<span data-ttu-id="8f991-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f991-116">Application</span></span>|<span data-ttu-id="8f991-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f991-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f991-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f991-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8f991-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f991-119">Request headers</span></span>
|<span data-ttu-id="8f991-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f991-120">Header</span></span>|<span data-ttu-id="8f991-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8f991-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f991-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f991-122">Authorization</span></span>|<span data-ttu-id="8f991-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f991-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f991-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8f991-124">Accept</span></span>|<span data-ttu-id="8f991-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f991-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f991-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f991-126">Request body</span></span>
<span data-ttu-id="8f991-127">В тексте запроса добавьте представление объекта [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f991-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="8f991-128">В следующей таблице приведены свойства, необходимые при создании [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="8f991-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="8f991-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f991-129">Property</span></span>|<span data-ttu-id="8f991-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f991-130">Type</span></span>|<span data-ttu-id="8f991-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f991-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f991-132">id</span><span class="sxs-lookup"><span data-stu-id="8f991-132">id</span></span>|<span data-ttu-id="8f991-133">String</span><span class="sxs-lookup"><span data-stu-id="8f991-133">String</span></span>|<span data-ttu-id="8f991-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f991-134">The key of the entity.</span></span>|
|<span data-ttu-id="8f991-135">content</span><span class="sxs-lookup"><span data-stu-id="8f991-135">content</span></span>|<span data-ttu-id="8f991-136">Binary</span><span class="sxs-lookup"><span data-stu-id="8f991-136">Binary</span></span>|<span data-ttu-id="8f991-137">Сертификат подписи кода Windows Symantec в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="8f991-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="8f991-138">status</span><span class="sxs-lookup"><span data-stu-id="8f991-138">status</span></span>|[<span data-ttu-id="8f991-139">Цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="8f991-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="8f991-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="8f991-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="8f991-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="8f991-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="8f991-142">password</span><span class="sxs-lookup"><span data-stu-id="8f991-142">password</span></span>|<span data-ttu-id="8f991-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8f991-143">String</span></span>|<span data-ttu-id="8f991-144">Пароль, необходимый для PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="8f991-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="8f991-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="8f991-145">subjectName</span></span>|<span data-ttu-id="8f991-146">String</span><span class="sxs-lookup"><span data-stu-id="8f991-146">String</span></span>|<span data-ttu-id="8f991-147">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="8f991-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="8f991-148">subject</span><span class="sxs-lookup"><span data-stu-id="8f991-148">subject</span></span>|<span data-ttu-id="8f991-149">String</span><span class="sxs-lookup"><span data-stu-id="8f991-149">String</span></span>|<span data-ttu-id="8f991-150">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="8f991-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="8f991-151">Иссуернаме</span><span class="sxs-lookup"><span data-stu-id="8f991-151">issuerName</span></span>|<span data-ttu-id="8f991-152">String</span><span class="sxs-lookup"><span data-stu-id="8f991-152">String</span></span>|<span data-ttu-id="8f991-153">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="8f991-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="8f991-154">имени</span><span class="sxs-lookup"><span data-stu-id="8f991-154">issuer</span></span>|<span data-ttu-id="8f991-155">String</span><span class="sxs-lookup"><span data-stu-id="8f991-155">String</span></span>|<span data-ttu-id="8f991-156">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="8f991-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="8f991-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8f991-157">expirationDateTime</span></span>|<span data-ttu-id="8f991-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f991-158">DateTimeOffset</span></span>|<span data-ttu-id="8f991-159">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8f991-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="8f991-160">Уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="8f991-160">uploadDateTime</span></span>|<span data-ttu-id="8f991-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f991-161">DateTimeOffset</span></span>|<span data-ttu-id="8f991-162">Тип сертификата соПроектировании в качестве сертификата Symantec.</span><span class="sxs-lookup"><span data-stu-id="8f991-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="8f991-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f991-163">Response</span></span>
<span data-ttu-id="8f991-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f991-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f991-165">Пример</span><span class="sxs-lookup"><span data-stu-id="8f991-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f991-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f991-166">Request</span></span>
<span data-ttu-id="8f991-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f991-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f991-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f991-168">Response</span></span>
<span data-ttu-id="8f991-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f991-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




