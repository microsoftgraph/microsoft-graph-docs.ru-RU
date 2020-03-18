---
title: Обновление Ентерприсекодесигнингцертификате
description: Обновление свойств объекта Ентерприсекодесигнингцертификате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccae1a99fae750808f8703bc8163738d4cf3ab84
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762128"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="31bca-103">Обновление Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="31bca-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="31bca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31bca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31bca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31bca-106">Обновление свойств объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="31bca-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31bca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31bca-107">Prerequisites</span></span>
<span data-ttu-id="31bca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31bca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31bca-110">Permission type</span></span>|<span data-ttu-id="31bca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31bca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31bca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31bca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31bca-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31bca-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31bca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31bca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31bca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bca-115">Not supported.</span></span>|
|<span data-ttu-id="31bca-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="31bca-116">Application</span></span>|<span data-ttu-id="31bca-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31bca-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31bca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31bca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="31bca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31bca-119">Request headers</span></span>
|<span data-ttu-id="31bca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31bca-120">Header</span></span>|<span data-ttu-id="31bca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31bca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31bca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31bca-122">Authorization</span></span>|<span data-ttu-id="31bca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31bca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31bca-124">Accept</span></span>|<span data-ttu-id="31bca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31bca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31bca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31bca-126">Request body</span></span>
<span data-ttu-id="31bca-127">В тексте запроса добавьте представление объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31bca-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="31bca-128">В следующей таблице приведены свойства, необходимые при создании [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="31bca-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="31bca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bca-129">Property</span></span>|<span data-ttu-id="31bca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31bca-130">Type</span></span>|<span data-ttu-id="31bca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31bca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31bca-132">id</span><span class="sxs-lookup"><span data-stu-id="31bca-132">id</span></span>|<span data-ttu-id="31bca-133">Строка</span><span class="sxs-lookup"><span data-stu-id="31bca-133">String</span></span>|<span data-ttu-id="31bca-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31bca-134">The key of the entity.</span></span>|
|<span data-ttu-id="31bca-135">содержимое</span><span class="sxs-lookup"><span data-stu-id="31bca-135">content</span></span>|<span data-ttu-id="31bca-136">Binary</span><span class="sxs-lookup"><span data-stu-id="31bca-136">Binary</span></span>|<span data-ttu-id="31bca-137">Сертификат подписи кода Windows Enterprise в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="31bca-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="31bca-138">status</span><span class="sxs-lookup"><span data-stu-id="31bca-138">status</span></span>|[<span data-ttu-id="31bca-139">цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="31bca-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="31bca-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="31bca-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="31bca-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="31bca-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="31bca-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="31bca-142">subjectName</span></span>|<span data-ttu-id="31bca-143">String</span><span class="sxs-lookup"><span data-stu-id="31bca-143">String</span></span>|<span data-ttu-id="31bca-144">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="31bca-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="31bca-145">subject</span><span class="sxs-lookup"><span data-stu-id="31bca-145">subject</span></span>|<span data-ttu-id="31bca-146">String</span><span class="sxs-lookup"><span data-stu-id="31bca-146">String</span></span>|<span data-ttu-id="31bca-147">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="31bca-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="31bca-148">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="31bca-148">issuerName</span></span>|<span data-ttu-id="31bca-149">String</span><span class="sxs-lookup"><span data-stu-id="31bca-149">String</span></span>|<span data-ttu-id="31bca-150">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="31bca-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="31bca-151">имени</span><span class="sxs-lookup"><span data-stu-id="31bca-151">issuer</span></span>|<span data-ttu-id="31bca-152">String</span><span class="sxs-lookup"><span data-stu-id="31bca-152">String</span></span>|<span data-ttu-id="31bca-153">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="31bca-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="31bca-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="31bca-154">expirationDateTime</span></span>|<span data-ttu-id="31bca-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31bca-155">DateTimeOffset</span></span>|<span data-ttu-id="31bca-156">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="31bca-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="31bca-157">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="31bca-157">uploadDateTime</span></span>|<span data-ttu-id="31bca-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31bca-158">DateTimeOffset</span></span>|<span data-ttu-id="31bca-159">Дата и время отправки сертификата соконструирования.</span><span class="sxs-lookup"><span data-stu-id="31bca-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="31bca-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="31bca-160">Response</span></span>
<span data-ttu-id="31bca-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31bca-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31bca-162">Пример</span><span class="sxs-lookup"><span data-stu-id="31bca-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="31bca-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bca-163">Request</span></span>
<span data-ttu-id="31bca-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31bca-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="31bca-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="31bca-165">Response</span></span>
<span data-ttu-id="31bca-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31bca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```




