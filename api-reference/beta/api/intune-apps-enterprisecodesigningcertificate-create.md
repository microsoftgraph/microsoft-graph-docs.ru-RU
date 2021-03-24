---
title: Создание enterpriseCodeSigningCertificate
description: Создание нового объекта enterpriseCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0c5d96d6e5362866c279211f4252bd9cd544c1e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144292"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="850bb-103">Создание enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="850bb-103">Create enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="850bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="850bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="850bb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="850bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="850bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="850bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="850bb-107">Создание нового [объекта enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="850bb-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="850bb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="850bb-108">Prerequisites</span></span>
<span data-ttu-id="850bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="850bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="850bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="850bb-111">Permission type</span></span>|<span data-ttu-id="850bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="850bb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="850bb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="850bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="850bb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850bb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="850bb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="850bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="850bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="850bb-116">Not supported.</span></span>|
|<span data-ttu-id="850bb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="850bb-117">Application</span></span>|<span data-ttu-id="850bb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850bb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="850bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="850bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="850bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="850bb-120">Request headers</span></span>
|<span data-ttu-id="850bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="850bb-121">Header</span></span>|<span data-ttu-id="850bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="850bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="850bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="850bb-123">Authorization</span></span>|<span data-ttu-id="850bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="850bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="850bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="850bb-125">Accept</span></span>|<span data-ttu-id="850bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="850bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="850bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="850bb-127">Request body</span></span>
<span data-ttu-id="850bb-128">В теле запроса поставляем представление JSON для объекта enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="850bb-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="850bb-129">В следующей таблице показаны свойства, необходимые при создании enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="850bb-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="850bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="850bb-130">Property</span></span>|<span data-ttu-id="850bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="850bb-131">Type</span></span>|<span data-ttu-id="850bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="850bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="850bb-133">id</span><span class="sxs-lookup"><span data-stu-id="850bb-133">id</span></span>|<span data-ttu-id="850bb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="850bb-134">String</span></span>|<span data-ttu-id="850bb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="850bb-135">The key of the entity.</span></span>|
|<span data-ttu-id="850bb-136">содержимое</span><span class="sxs-lookup"><span data-stu-id="850bb-136">content</span></span>|<span data-ttu-id="850bb-137">Binary</span><span class="sxs-lookup"><span data-stu-id="850bb-137">Binary</span></span>|<span data-ttu-id="850bb-138">Сертификат предприятия Windows Code-Signing в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="850bb-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="850bb-139">status</span><span class="sxs-lookup"><span data-stu-id="850bb-139">status</span></span>|[<span data-ttu-id="850bb-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="850bb-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="850bb-141">Состояние сертификата, предварительное или не предварительное.</span><span class="sxs-lookup"><span data-stu-id="850bb-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="850bb-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="850bb-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="850bb-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="850bb-143">subjectName</span></span>|<span data-ttu-id="850bb-144">String</span><span class="sxs-lookup"><span data-stu-id="850bb-144">String</span></span>|<span data-ttu-id="850bb-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="850bb-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="850bb-146">subject</span><span class="sxs-lookup"><span data-stu-id="850bb-146">subject</span></span>|<span data-ttu-id="850bb-147">String</span><span class="sxs-lookup"><span data-stu-id="850bb-147">String</span></span>|<span data-ttu-id="850bb-148">Значение subject для сертификата.</span><span class="sxs-lookup"><span data-stu-id="850bb-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="850bb-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="850bb-149">issuerName</span></span>|<span data-ttu-id="850bb-150">Строка</span><span class="sxs-lookup"><span data-stu-id="850bb-150">String</span></span>|<span data-ttu-id="850bb-151">Имя эмитента для сертификата.</span><span class="sxs-lookup"><span data-stu-id="850bb-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="850bb-152">эмитент</span><span class="sxs-lookup"><span data-stu-id="850bb-152">issuer</span></span>|<span data-ttu-id="850bb-153">Строка</span><span class="sxs-lookup"><span data-stu-id="850bb-153">String</span></span>|<span data-ttu-id="850bb-154">Значение Issuer для сертификата.</span><span class="sxs-lookup"><span data-stu-id="850bb-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="850bb-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="850bb-155">expirationDateTime</span></span>|<span data-ttu-id="850bb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="850bb-156">DateTimeOffset</span></span>|<span data-ttu-id="850bb-157">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="850bb-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="850bb-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="850bb-158">uploadDateTime</span></span>|<span data-ttu-id="850bb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="850bb-159">DateTimeOffset</span></span>|<span data-ttu-id="850bb-160">Время даты отправки сертификата CodeSigning.</span><span class="sxs-lookup"><span data-stu-id="850bb-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="850bb-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="850bb-161">Response</span></span>
<span data-ttu-id="850bb-162">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="850bb-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="850bb-163">Пример</span><span class="sxs-lookup"><span data-stu-id="850bb-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="850bb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="850bb-164">Request</span></span>
<span data-ttu-id="850bb-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="850bb-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
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

### <a name="response"></a><span data-ttu-id="850bb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="850bb-166">Response</span></span>
<span data-ttu-id="850bb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="850bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




