---
title: Обновление Ентерприсекодесигнингцертификате
description: Обновление свойств объекта Ентерприсекодесигнингцертификате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fad5751730adb14516dad0688369495fd6061070
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252985"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="fdb5a-103">Обновление Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="fdb5a-103">Update enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="fdb5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdb5a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdb5a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdb5a-107">Обновление свойств объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="fdb5a-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdb5a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdb5a-108">Prerequisites</span></span>
<span data-ttu-id="fdb5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdb5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdb5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdb5a-111">Permission type</span></span>|<span data-ttu-id="fdb5a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdb5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdb5a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdb5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdb5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fdb5a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdb5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdb5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-116">Not supported.</span></span>|
|<span data-ttu-id="fdb5a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fdb5a-117">Application</span></span>|<span data-ttu-id="fdb5a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb5a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdb5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdb5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="fdb5a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fdb5a-120">Request headers</span></span>
|<span data-ttu-id="fdb5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdb5a-121">Header</span></span>|<span data-ttu-id="fdb5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdb5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdb5a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdb5a-123">Authorization</span></span>|<span data-ttu-id="fdb5a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdb5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdb5a-125">Accept</span></span>|<span data-ttu-id="fdb5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdb5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdb5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdb5a-127">Request body</span></span>
<span data-ttu-id="fdb5a-128">В тексте запроса добавьте представление объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="fdb5a-129">В следующей таблице приведены свойства, необходимые при создании [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="fdb5a-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="fdb5a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdb5a-130">Property</span></span>|<span data-ttu-id="fdb5a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdb5a-131">Type</span></span>|<span data-ttu-id="fdb5a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdb5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb5a-133">id</span><span class="sxs-lookup"><span data-stu-id="fdb5a-133">id</span></span>|<span data-ttu-id="fdb5a-134">String</span><span class="sxs-lookup"><span data-stu-id="fdb5a-134">String</span></span>|<span data-ttu-id="fdb5a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-135">The key of the entity.</span></span>|
|<span data-ttu-id="fdb5a-136">содержимое</span><span class="sxs-lookup"><span data-stu-id="fdb5a-136">content</span></span>|<span data-ttu-id="fdb5a-137">Binary</span><span class="sxs-lookup"><span data-stu-id="fdb5a-137">Binary</span></span>|<span data-ttu-id="fdb5a-138">Сертификат Windows корпоративный Code-Signing в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="fdb5a-139">status</span><span class="sxs-lookup"><span data-stu-id="fdb5a-139">status</span></span>|[<span data-ttu-id="fdb5a-140">цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="fdb5a-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="fdb5a-141">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="fdb5a-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="fdb5a-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="fdb5a-143">subjectName</span></span>|<span data-ttu-id="fdb5a-144">String</span><span class="sxs-lookup"><span data-stu-id="fdb5a-144">String</span></span>|<span data-ttu-id="fdb5a-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="fdb5a-146">subject</span><span class="sxs-lookup"><span data-stu-id="fdb5a-146">subject</span></span>|<span data-ttu-id="fdb5a-147">String</span><span class="sxs-lookup"><span data-stu-id="fdb5a-147">String</span></span>|<span data-ttu-id="fdb5a-148">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="fdb5a-149">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="fdb5a-149">issuerName</span></span>|<span data-ttu-id="fdb5a-150">String</span><span class="sxs-lookup"><span data-stu-id="fdb5a-150">String</span></span>|<span data-ttu-id="fdb5a-151">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="fdb5a-152">имени</span><span class="sxs-lookup"><span data-stu-id="fdb5a-152">issuer</span></span>|<span data-ttu-id="fdb5a-153">String</span><span class="sxs-lookup"><span data-stu-id="fdb5a-153">String</span></span>|<span data-ttu-id="fdb5a-154">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="fdb5a-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fdb5a-155">expirationDateTime</span></span>|<span data-ttu-id="fdb5a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdb5a-156">DateTimeOffset</span></span>|<span data-ttu-id="fdb5a-157">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="fdb5a-158">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="fdb5a-158">uploadDateTime</span></span>|<span data-ttu-id="fdb5a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdb5a-159">DateTimeOffset</span></span>|<span data-ttu-id="fdb5a-160">Дата и время отправки сертификата соконструирования.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="fdb5a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdb5a-161">Response</span></span>
<span data-ttu-id="fdb5a-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdb5a-163">Пример</span><span class="sxs-lookup"><span data-stu-id="fdb5a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdb5a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdb5a-164">Request</span></span>
<span data-ttu-id="fdb5a-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdb5a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdb5a-166">Response</span></span>
<span data-ttu-id="fdb5a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdb5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




