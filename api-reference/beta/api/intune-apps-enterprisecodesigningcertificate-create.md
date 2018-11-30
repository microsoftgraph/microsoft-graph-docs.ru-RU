---
title: Создание enterpriseCodeSigningCertificate
description: Создание нового объекта enterpriseCodeSigningCertificate.
ms.openlocfilehash: aa5d92c22a1cd4eb91a41b26ed92f76937ce9dcd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074665"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="c7e31-103">Создание enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c7e31-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="c7e31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7e31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7e31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7e31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c7e31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7e31-107">Создание нового объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c7e31-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7e31-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7e31-108">Prerequisites</span></span>
<span data-ttu-id="c7e31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e31-111">Permission type</span></span>|<span data-ttu-id="c7e31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7e31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7e31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7e31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7e31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7e31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7e31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7e31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e31-116">Not supported.</span></span>|
|<span data-ttu-id="c7e31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7e31-117">Application</span></span>|<span data-ttu-id="c7e31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7e31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="c7e31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7e31-120">Request headers</span></span>
|<span data-ttu-id="c7e31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7e31-121">Header</span></span>|<span data-ttu-id="c7e31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7e31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7e31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e31-123">Authorization</span></span>|<span data-ttu-id="c7e31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7e31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7e31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7e31-125">Accept</span></span>|<span data-ttu-id="c7e31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7e31-127">Request body</span></span>
<span data-ttu-id="c7e31-128">В тексте запроса укажите представление JSON для объекта enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="c7e31-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="c7e31-129">В следующей таблице показаны свойства, которые необходимы для создания enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="c7e31-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="c7e31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7e31-130">Property</span></span>|<span data-ttu-id="c7e31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7e31-131">Type</span></span>|<span data-ttu-id="c7e31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e31-133">id</span><span class="sxs-lookup"><span data-stu-id="c7e31-133">id</span></span>|<span data-ttu-id="c7e31-134">String</span><span class="sxs-lookup"><span data-stu-id="c7e31-134">String</span></span>|<span data-ttu-id="c7e31-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7e31-135">The key of the entity.</span></span>|
|<span data-ttu-id="c7e31-136">content</span><span class="sxs-lookup"><span data-stu-id="c7e31-136">content</span></span>|<span data-ttu-id="c7e31-137">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c7e31-137">Binary</span></span>|<span data-ttu-id="c7e31-138">Сертификат подписи кода Enterprise Windows в формате необработанные данные.</span><span class="sxs-lookup"><span data-stu-id="c7e31-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c7e31-139">status</span><span class="sxs-lookup"><span data-stu-id="c7e31-139">status</span></span>|[<span data-ttu-id="c7e31-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c7e31-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c7e31-141">Состояние сертификата подготовить к работе или не подготовлен.</span><span class="sxs-lookup"><span data-stu-id="c7e31-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c7e31-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="c7e31-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c7e31-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="c7e31-143">subjectName</span></span>|<span data-ttu-id="c7e31-144">String</span><span class="sxs-lookup"><span data-stu-id="c7e31-144">String</span></span>|<span data-ttu-id="c7e31-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7e31-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c7e31-146">subject</span><span class="sxs-lookup"><span data-stu-id="c7e31-146">subject</span></span>|<span data-ttu-id="c7e31-147">String</span><span class="sxs-lookup"><span data-stu-id="c7e31-147">String</span></span>|<span data-ttu-id="c7e31-148">Значения субъектов для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7e31-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="c7e31-149">Имя поставщика</span><span class="sxs-lookup"><span data-stu-id="c7e31-149">issuerName</span></span>|<span data-ttu-id="c7e31-150">String</span><span class="sxs-lookup"><span data-stu-id="c7e31-150">String</span></span>|<span data-ttu-id="c7e31-151">Имя поставщика для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7e31-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c7e31-152">издателя</span><span class="sxs-lookup"><span data-stu-id="c7e31-152">issuer</span></span>|<span data-ttu-id="c7e31-153">String</span><span class="sxs-lookup"><span data-stu-id="c7e31-153">String</span></span>|<span data-ttu-id="c7e31-154">Значение издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7e31-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c7e31-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c7e31-155">expirationDateTime</span></span>|<span data-ttu-id="c7e31-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7e31-156">DateTimeOffset</span></span>|<span data-ttu-id="c7e31-157">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7e31-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c7e31-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c7e31-158">uploadDateTime</span></span>|<span data-ttu-id="c7e31-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7e31-159">DateTimeOffset</span></span>|<span data-ttu-id="c7e31-160">Дата время подписывания кода сертификата при его загрузке.</span><span class="sxs-lookup"><span data-stu-id="c7e31-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="c7e31-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7e31-161">Response</span></span>
<span data-ttu-id="c7e31-162">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7e31-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e31-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c7e31-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7e31-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7e31-164">Request</span></span>
<span data-ttu-id="c7e31-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7e31-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7e31-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7e31-166">Response</span></span>
<span data-ttu-id="c7e31-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c7e31-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





