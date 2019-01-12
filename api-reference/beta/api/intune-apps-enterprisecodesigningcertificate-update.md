---
title: Обновление enterpriseCodeSigningCertificate
description: Обновление свойства объекта enterpriseCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5133f5dffa98834ce44849c6b18c73cc19732756
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955116"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="12cce-103">Обновление enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="12cce-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="12cce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12cce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12cce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12cce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12cce-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12cce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12cce-107">Обновление свойства объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="12cce-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12cce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12cce-108">Prerequisites</span></span>
<span data-ttu-id="12cce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12cce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12cce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12cce-111">Permission type</span></span>|<span data-ttu-id="12cce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12cce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12cce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12cce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12cce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12cce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12cce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12cce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12cce-116">Not supported.</span></span>|
|<span data-ttu-id="12cce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12cce-117">Application</span></span>|<span data-ttu-id="12cce-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12cce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12cce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12cce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="12cce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12cce-120">Request headers</span></span>
|<span data-ttu-id="12cce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12cce-121">Header</span></span>|<span data-ttu-id="12cce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12cce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12cce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12cce-123">Authorization</span></span>|<span data-ttu-id="12cce-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12cce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12cce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12cce-125">Accept</span></span>|<span data-ttu-id="12cce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12cce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12cce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12cce-127">Request body</span></span>
<span data-ttu-id="12cce-128">В тексте запроса укажите представление JSON для объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="12cce-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="12cce-129">В следующей таблице показаны свойства, которые необходимы для создания [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="12cce-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="12cce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12cce-130">Property</span></span>|<span data-ttu-id="12cce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12cce-131">Type</span></span>|<span data-ttu-id="12cce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12cce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cce-133">id</span><span class="sxs-lookup"><span data-stu-id="12cce-133">id</span></span>|<span data-ttu-id="12cce-134">String</span><span class="sxs-lookup"><span data-stu-id="12cce-134">String</span></span>|<span data-ttu-id="12cce-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12cce-135">The key of the entity.</span></span>|
|<span data-ttu-id="12cce-136">content</span><span class="sxs-lookup"><span data-stu-id="12cce-136">content</span></span>|<span data-ttu-id="12cce-137">Binary</span><span class="sxs-lookup"><span data-stu-id="12cce-137">Binary</span></span>|<span data-ttu-id="12cce-138">Сертификат подписи кода Enterprise Windows в формате необработанные данные.</span><span class="sxs-lookup"><span data-stu-id="12cce-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="12cce-139">status</span><span class="sxs-lookup"><span data-stu-id="12cce-139">status</span></span>|[<span data-ttu-id="12cce-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="12cce-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="12cce-141">Состояние сертификата подготовить к работе или не подготовлен.</span><span class="sxs-lookup"><span data-stu-id="12cce-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="12cce-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="12cce-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="12cce-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="12cce-143">subjectName</span></span>|<span data-ttu-id="12cce-144">String</span><span class="sxs-lookup"><span data-stu-id="12cce-144">String</span></span>|<span data-ttu-id="12cce-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="12cce-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="12cce-146">subject</span><span class="sxs-lookup"><span data-stu-id="12cce-146">subject</span></span>|<span data-ttu-id="12cce-147">String</span><span class="sxs-lookup"><span data-stu-id="12cce-147">String</span></span>|<span data-ttu-id="12cce-148">Значения субъектов для сертификата.</span><span class="sxs-lookup"><span data-stu-id="12cce-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="12cce-149">Имя поставщика</span><span class="sxs-lookup"><span data-stu-id="12cce-149">issuerName</span></span>|<span data-ttu-id="12cce-150">String</span><span class="sxs-lookup"><span data-stu-id="12cce-150">String</span></span>|<span data-ttu-id="12cce-151">Имя поставщика для сертификата.</span><span class="sxs-lookup"><span data-stu-id="12cce-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="12cce-152">издателя</span><span class="sxs-lookup"><span data-stu-id="12cce-152">issuer</span></span>|<span data-ttu-id="12cce-153">String</span><span class="sxs-lookup"><span data-stu-id="12cce-153">String</span></span>|<span data-ttu-id="12cce-154">Значение издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="12cce-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="12cce-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="12cce-155">expirationDateTime</span></span>|<span data-ttu-id="12cce-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12cce-156">DateTimeOffset</span></span>|<span data-ttu-id="12cce-157">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="12cce-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="12cce-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="12cce-158">uploadDateTime</span></span>|<span data-ttu-id="12cce-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12cce-159">DateTimeOffset</span></span>|<span data-ttu-id="12cce-160">Дата время подписывания кода сертификата при его загрузке.</span><span class="sxs-lookup"><span data-stu-id="12cce-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="12cce-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="12cce-161">Response</span></span>
<span data-ttu-id="12cce-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12cce-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12cce-163">Пример</span><span class="sxs-lookup"><span data-stu-id="12cce-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="12cce-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="12cce-164">Request</span></span>
<span data-ttu-id="12cce-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12cce-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 319

{
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

### <a name="response"></a><span data-ttu-id="12cce-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="12cce-166">Response</span></span>
<span data-ttu-id="12cce-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12cce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





