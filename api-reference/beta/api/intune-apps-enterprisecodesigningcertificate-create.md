---
title: Создание Ентерприсекодесигнингцертификате
description: Создание нового объекта Ентерприсекодесигнингцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce8700728284af5d2092d6fa6b3057368106eb6e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975240"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="537c0-103">Создание Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="537c0-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="537c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="537c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="537c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="537c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="537c0-106">Создание нового объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="537c0-106">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="537c0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="537c0-107">Prerequisites</span></span>
<span data-ttu-id="537c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="537c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="537c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="537c0-110">Permission type</span></span>|<span data-ttu-id="537c0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="537c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="537c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="537c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="537c0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537c0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="537c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="537c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="537c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="537c0-115">Not supported.</span></span>|
|<span data-ttu-id="537c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="537c0-116">Application</span></span>|<span data-ttu-id="537c0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="537c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="537c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="537c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="537c0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="537c0-119">Request headers</span></span>
|<span data-ttu-id="537c0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="537c0-120">Header</span></span>|<span data-ttu-id="537c0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="537c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="537c0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="537c0-122">Authorization</span></span>|<span data-ttu-id="537c0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="537c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="537c0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="537c0-124">Accept</span></span>|<span data-ttu-id="537c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="537c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="537c0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="537c0-126">Request body</span></span>
<span data-ttu-id="537c0-127">В тексте запроса добавьте представление объекта Ентерприсекодесигнингцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="537c0-127">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="537c0-128">В следующей таблице приведены свойства, необходимые при создании Ентерприсекодесигнингцертификате.</span><span class="sxs-lookup"><span data-stu-id="537c0-128">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="537c0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="537c0-129">Property</span></span>|<span data-ttu-id="537c0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="537c0-130">Type</span></span>|<span data-ttu-id="537c0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="537c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="537c0-132">id</span><span class="sxs-lookup"><span data-stu-id="537c0-132">id</span></span>|<span data-ttu-id="537c0-133">String</span><span class="sxs-lookup"><span data-stu-id="537c0-133">String</span></span>|<span data-ttu-id="537c0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="537c0-134">The key of the entity.</span></span>|
|<span data-ttu-id="537c0-135">содержимое</span><span class="sxs-lookup"><span data-stu-id="537c0-135">content</span></span>|<span data-ttu-id="537c0-136">Binary</span><span class="sxs-lookup"><span data-stu-id="537c0-136">Binary</span></span>|<span data-ttu-id="537c0-137">Сертификат подписи кода Windows Enterprise в формате необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="537c0-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="537c0-138">status</span><span class="sxs-lookup"><span data-stu-id="537c0-138">status</span></span>|[<span data-ttu-id="537c0-139">Цертификатестатус</span><span class="sxs-lookup"><span data-stu-id="537c0-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="537c0-140">Состояние сертификата подготовлено или не подготовлено.</span><span class="sxs-lookup"><span data-stu-id="537c0-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="537c0-141">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="537c0-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="537c0-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="537c0-142">subjectName</span></span>|<span data-ttu-id="537c0-143">String</span><span class="sxs-lookup"><span data-stu-id="537c0-143">String</span></span>|<span data-ttu-id="537c0-144">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="537c0-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="537c0-145">subject</span><span class="sxs-lookup"><span data-stu-id="537c0-145">subject</span></span>|<span data-ttu-id="537c0-146">String</span><span class="sxs-lookup"><span data-stu-id="537c0-146">String</span></span>|<span data-ttu-id="537c0-147">Значение субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="537c0-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="537c0-148">Иссуернаме</span><span class="sxs-lookup"><span data-stu-id="537c0-148">issuerName</span></span>|<span data-ttu-id="537c0-149">String</span><span class="sxs-lookup"><span data-stu-id="537c0-149">String</span></span>|<span data-ttu-id="537c0-150">Имя поставщика сертификата.</span><span class="sxs-lookup"><span data-stu-id="537c0-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="537c0-151">имени</span><span class="sxs-lookup"><span data-stu-id="537c0-151">issuer</span></span>|<span data-ttu-id="537c0-152">String</span><span class="sxs-lookup"><span data-stu-id="537c0-152">String</span></span>|<span data-ttu-id="537c0-153">Значение издателя для сертификата.</span><span class="sxs-lookup"><span data-stu-id="537c0-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="537c0-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="537c0-154">expirationDateTime</span></span>|<span data-ttu-id="537c0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537c0-155">DateTimeOffset</span></span>|<span data-ttu-id="537c0-156">Дата окончания срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="537c0-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="537c0-157">Уплоаддатетиме</span><span class="sxs-lookup"><span data-stu-id="537c0-157">uploadDateTime</span></span>|<span data-ttu-id="537c0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537c0-158">DateTimeOffset</span></span>|<span data-ttu-id="537c0-159">Дата и время отправки сертификата соКонструирования.</span><span class="sxs-lookup"><span data-stu-id="537c0-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="537c0-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="537c0-160">Response</span></span>
<span data-ttu-id="537c0-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="537c0-161">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="537c0-162">Пример</span><span class="sxs-lookup"><span data-stu-id="537c0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="537c0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="537c0-163">Request</span></span>
<span data-ttu-id="537c0-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="537c0-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="537c0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="537c0-165">Response</span></span>
<span data-ttu-id="537c0-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="537c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




