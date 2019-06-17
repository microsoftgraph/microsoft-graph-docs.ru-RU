---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойств объекта symantecCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32b7d60ae97160a134e6ac26d640a545bb7a429a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973497"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="dcffb-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="dcffb-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="dcffb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcffb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcffb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcffb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcffb-106">Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="dcffb-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcffb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dcffb-107">Prerequisites</span></span>
<span data-ttu-id="dcffb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcffb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcffb-110">Permission type</span></span>|<span data-ttu-id="dcffb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcffb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcffb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcffb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcffb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcffb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dcffb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcffb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcffb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcffb-115">Not supported.</span></span>|
|<span data-ttu-id="dcffb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcffb-116">Application</span></span>|<span data-ttu-id="dcffb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcffb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcffb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcffb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="dcffb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcffb-119">Request headers</span></span>
|<span data-ttu-id="dcffb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcffb-120">Header</span></span>|<span data-ttu-id="dcffb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dcffb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcffb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcffb-122">Authorization</span></span>|<span data-ttu-id="dcffb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcffb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcffb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dcffb-124">Accept</span></span>|<span data-ttu-id="dcffb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcffb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcffb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dcffb-126">Request body</span></span>
<span data-ttu-id="dcffb-127">В тексте запроса добавьте представление объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcffb-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="dcffb-128">В следующей таблице приведены свойства, необходимые при создании [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="dcffb-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="dcffb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcffb-129">Property</span></span>|<span data-ttu-id="dcffb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dcffb-130">Type</span></span>|<span data-ttu-id="dcffb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dcffb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcffb-132">id</span><span class="sxs-lookup"><span data-stu-id="dcffb-132">id</span></span>|<span data-ttu-id="dcffb-133">String</span><span class="sxs-lookup"><span data-stu-id="dcffb-133">String</span></span>|<span data-ttu-id="dcffb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dcffb-134">The key of the entity.</span></span>|
|<span data-ttu-id="dcffb-135">содержимое</span><span class="sxs-lookup"><span data-stu-id="dcffb-135">content</span></span>|<span data-ttu-id="dcffb-136">Binary</span><span class="sxs-lookup"><span data-stu-id="dcffb-136">Binary</span></span>|<span data-ttu-id="dcffb-137">Сертификат подписи кода Windows Symantec в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="dcffb-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="dcffb-138">status</span><span class="sxs-lookup"><span data-stu-id="dcffb-138">status</span></span>|[<span data-ttu-id="dcffb-139">Цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="dcffb-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="dcffb-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="dcffb-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="dcffb-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="dcffb-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="dcffb-142">password</span><span class="sxs-lookup"><span data-stu-id="dcffb-142">password</span></span>|<span data-ttu-id="dcffb-143">Строка</span><span class="sxs-lookup"><span data-stu-id="dcffb-143">String</span></span>|<span data-ttu-id="dcffb-144">Пароль, необходимый для PFX-файла.</span><span class="sxs-lookup"><span data-stu-id="dcffb-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="dcffb-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="dcffb-145">subjectName</span></span>|<span data-ttu-id="dcffb-146">String</span><span class="sxs-lookup"><span data-stu-id="dcffb-146">String</span></span>|<span data-ttu-id="dcffb-147">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcffb-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="dcffb-148">subject</span><span class="sxs-lookup"><span data-stu-id="dcffb-148">subject</span></span>|<span data-ttu-id="dcffb-149">String</span><span class="sxs-lookup"><span data-stu-id="dcffb-149">String</span></span>|<span data-ttu-id="dcffb-150">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcffb-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="dcffb-151">Иссуернаме</span><span class="sxs-lookup"><span data-stu-id="dcffb-151">issuerName</span></span>|<span data-ttu-id="dcffb-152">String</span><span class="sxs-lookup"><span data-stu-id="dcffb-152">String</span></span>|<span data-ttu-id="dcffb-153">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcffb-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="dcffb-154">имени</span><span class="sxs-lookup"><span data-stu-id="dcffb-154">issuer</span></span>|<span data-ttu-id="dcffb-155">String</span><span class="sxs-lookup"><span data-stu-id="dcffb-155">String</span></span>|<span data-ttu-id="dcffb-156">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcffb-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="dcffb-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dcffb-157">expirationDateTime</span></span>|<span data-ttu-id="dcffb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcffb-158">DateTimeOffset</span></span>|<span data-ttu-id="dcffb-159">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="dcffb-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="dcffb-160">Уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="dcffb-160">uploadDateTime</span></span>|<span data-ttu-id="dcffb-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcffb-161">DateTimeOffset</span></span>|<span data-ttu-id="dcffb-162">Тип сертификата сопроектировании в качестве сертификата Symantec.</span><span class="sxs-lookup"><span data-stu-id="dcffb-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="dcffb-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcffb-163">Response</span></span>
<span data-ttu-id="dcffb-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcffb-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcffb-165">Пример</span><span class="sxs-lookup"><span data-stu-id="dcffb-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcffb-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcffb-166">Request</span></span>
<span data-ttu-id="dcffb-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcffb-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dcffb-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcffb-168">Response</span></span>
<span data-ttu-id="dcffb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcffb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





