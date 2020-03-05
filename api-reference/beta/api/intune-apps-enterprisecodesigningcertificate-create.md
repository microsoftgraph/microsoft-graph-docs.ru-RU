---
title: Создание Ентерприсекодесигнингцертификате
description: Создание нового объекта Ентерприсекодесигнингцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f50b72b586f7e91a6f336a34c4c94e8aa093bbe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445787"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="f289c-103">Создание Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="f289c-103">Create enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="f289c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f289c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f289c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f289c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f289c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f289c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f289c-107">Создание нового объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="f289c-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f289c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f289c-108">Prerequisites</span></span>
<span data-ttu-id="f289c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f289c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f289c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f289c-111">Permission type</span></span>|<span data-ttu-id="f289c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f289c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f289c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f289c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f289c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f289c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f289c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f289c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f289c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f289c-116">Not supported.</span></span>|
|<span data-ttu-id="f289c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f289c-117">Application</span></span>|<span data-ttu-id="f289c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f289c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f289c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f289c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="f289c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f289c-120">Request headers</span></span>
|<span data-ttu-id="f289c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f289c-121">Header</span></span>|<span data-ttu-id="f289c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f289c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f289c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f289c-123">Authorization</span></span>|<span data-ttu-id="f289c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f289c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f289c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f289c-125">Accept</span></span>|<span data-ttu-id="f289c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f289c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f289c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f289c-127">Request body</span></span>
<span data-ttu-id="f289c-128">В тексте запроса добавьте представление объекта Ентерприсекодесигнингцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f289c-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="f289c-129">В следующей таблице приведены свойства, необходимые при создании Ентерприсекодесигнингцертификате.</span><span class="sxs-lookup"><span data-stu-id="f289c-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="f289c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f289c-130">Property</span></span>|<span data-ttu-id="f289c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f289c-131">Type</span></span>|<span data-ttu-id="f289c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f289c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f289c-133">id</span><span class="sxs-lookup"><span data-stu-id="f289c-133">id</span></span>|<span data-ttu-id="f289c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f289c-134">String</span></span>|<span data-ttu-id="f289c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f289c-135">The key of the entity.</span></span>|
|<span data-ttu-id="f289c-136">содержимое</span><span class="sxs-lookup"><span data-stu-id="f289c-136">content</span></span>|<span data-ttu-id="f289c-137">Binary</span><span class="sxs-lookup"><span data-stu-id="f289c-137">Binary</span></span>|<span data-ttu-id="f289c-138">Сертификат подписи кода Windows Enterprise в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="f289c-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="f289c-139">status</span><span class="sxs-lookup"><span data-stu-id="f289c-139">status</span></span>|[<span data-ttu-id="f289c-140">цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="f289c-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="f289c-141">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="f289c-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="f289c-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="f289c-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="f289c-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="f289c-143">subjectName</span></span>|<span data-ttu-id="f289c-144">String</span><span class="sxs-lookup"><span data-stu-id="f289c-144">String</span></span>|<span data-ttu-id="f289c-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="f289c-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="f289c-146">subject</span><span class="sxs-lookup"><span data-stu-id="f289c-146">subject</span></span>|<span data-ttu-id="f289c-147">String</span><span class="sxs-lookup"><span data-stu-id="f289c-147">String</span></span>|<span data-ttu-id="f289c-148">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="f289c-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="f289c-149">иссуернаме</span><span class="sxs-lookup"><span data-stu-id="f289c-149">issuerName</span></span>|<span data-ttu-id="f289c-150">String</span><span class="sxs-lookup"><span data-stu-id="f289c-150">String</span></span>|<span data-ttu-id="f289c-151">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="f289c-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="f289c-152">имени</span><span class="sxs-lookup"><span data-stu-id="f289c-152">issuer</span></span>|<span data-ttu-id="f289c-153">String</span><span class="sxs-lookup"><span data-stu-id="f289c-153">String</span></span>|<span data-ttu-id="f289c-154">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="f289c-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="f289c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f289c-155">expirationDateTime</span></span>|<span data-ttu-id="f289c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f289c-156">DateTimeOffset</span></span>|<span data-ttu-id="f289c-157">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f289c-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="f289c-158">уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="f289c-158">uploadDateTime</span></span>|<span data-ttu-id="f289c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f289c-159">DateTimeOffset</span></span>|<span data-ttu-id="f289c-160">Дата и время отправки сертификата соконструирования.</span><span class="sxs-lookup"><span data-stu-id="f289c-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="f289c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f289c-161">Response</span></span>
<span data-ttu-id="f289c-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f289c-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f289c-163">Пример</span><span class="sxs-lookup"><span data-stu-id="f289c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f289c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f289c-164">Request</span></span>
<span data-ttu-id="f289c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f289c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f289c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f289c-166">Response</span></span>
<span data-ttu-id="f289c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f289c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





