---
title: Создание Ентерприсекодесигнингцертификате
description: Создание нового объекта Ентерприсекодесигнингцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20b65d8b1eda5eab4bdd3e497eb6d505753f04de
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173103"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="ac394-103">Создание Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="ac394-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="ac394-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac394-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac394-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac394-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac394-106">Создание нового объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ac394-106">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac394-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ac394-107">Prerequisites</span></span>
<span data-ttu-id="ac394-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ac394-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac394-110">Permission type</span></span>|<span data-ttu-id="ac394-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac394-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac394-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac394-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac394-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac394-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac394-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac394-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac394-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac394-115">Not supported.</span></span>|
|<span data-ttu-id="ac394-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac394-116">Application</span></span>|<span data-ttu-id="ac394-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac394-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac394-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac394-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ac394-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac394-119">Request headers</span></span>
|<span data-ttu-id="ac394-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac394-120">Header</span></span>|<span data-ttu-id="ac394-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ac394-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac394-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac394-122">Authorization</span></span>|<span data-ttu-id="ac394-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ac394-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac394-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ac394-124">Accept</span></span>|<span data-ttu-id="ac394-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac394-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac394-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac394-126">Request body</span></span>
<span data-ttu-id="ac394-127">В тексте запроса добавьте представление объекта Ентерприсекодесигнингцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac394-127">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="ac394-128">В следующей таблице приведены свойства, необходимые при создании Ентерприсекодесигнингцертификате.</span><span class="sxs-lookup"><span data-stu-id="ac394-128">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="ac394-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac394-129">Property</span></span>|<span data-ttu-id="ac394-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ac394-130">Type</span></span>|<span data-ttu-id="ac394-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ac394-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac394-132">id</span><span class="sxs-lookup"><span data-stu-id="ac394-132">id</span></span>|<span data-ttu-id="ac394-133">String</span><span class="sxs-lookup"><span data-stu-id="ac394-133">String</span></span>|<span data-ttu-id="ac394-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ac394-134">The key of the entity.</span></span>|
|<span data-ttu-id="ac394-135">content</span><span class="sxs-lookup"><span data-stu-id="ac394-135">content</span></span>|<span data-ttu-id="ac394-136">Binary</span><span class="sxs-lookup"><span data-stu-id="ac394-136">Binary</span></span>|<span data-ttu-id="ac394-137">Сертификат подписи кода Windows Enterprise в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="ac394-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="ac394-138">status</span><span class="sxs-lookup"><span data-stu-id="ac394-138">status</span></span>|[<span data-ttu-id="ac394-139">Цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="ac394-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="ac394-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="ac394-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="ac394-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="ac394-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="ac394-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="ac394-142">subjectName</span></span>|<span data-ttu-id="ac394-143">String</span><span class="sxs-lookup"><span data-stu-id="ac394-143">String</span></span>|<span data-ttu-id="ac394-144">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="ac394-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="ac394-145">subject</span><span class="sxs-lookup"><span data-stu-id="ac394-145">subject</span></span>|<span data-ttu-id="ac394-146">String</span><span class="sxs-lookup"><span data-stu-id="ac394-146">String</span></span>|<span data-ttu-id="ac394-147">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="ac394-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="ac394-148">Иссуернаме</span><span class="sxs-lookup"><span data-stu-id="ac394-148">issuerName</span></span>|<span data-ttu-id="ac394-149">String</span><span class="sxs-lookup"><span data-stu-id="ac394-149">String</span></span>|<span data-ttu-id="ac394-150">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="ac394-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="ac394-151">имени</span><span class="sxs-lookup"><span data-stu-id="ac394-151">issuer</span></span>|<span data-ttu-id="ac394-152">String</span><span class="sxs-lookup"><span data-stu-id="ac394-152">String</span></span>|<span data-ttu-id="ac394-153">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="ac394-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="ac394-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ac394-154">expirationDateTime</span></span>|<span data-ttu-id="ac394-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac394-155">DateTimeOffset</span></span>|<span data-ttu-id="ac394-156">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ac394-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="ac394-157">Уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="ac394-157">uploadDateTime</span></span>|<span data-ttu-id="ac394-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac394-158">DateTimeOffset</span></span>|<span data-ttu-id="ac394-159">Дата и время отправки сертификата соКонструирования.</span><span class="sxs-lookup"><span data-stu-id="ac394-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="ac394-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac394-160">Response</span></span>
<span data-ttu-id="ac394-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac394-161">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac394-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ac394-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac394-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac394-163">Request</span></span>
<span data-ttu-id="ac394-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac394-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac394-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac394-165">Response</span></span>
<span data-ttu-id="ac394-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac394-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




