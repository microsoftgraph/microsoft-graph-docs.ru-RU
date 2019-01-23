---
title: Создание enterpriseCodeSigningCertificate
description: Создание нового объекта enterpriseCodeSigningCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ba50739903fce6e462f5c1a2602a4a61221eb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402554"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="01cfa-103">Создание enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="01cfa-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="01cfa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01cfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01cfa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01cfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01cfa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01cfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01cfa-107">Создание нового объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="01cfa-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01cfa-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="01cfa-108">Prerequisites</span></span>
<span data-ttu-id="01cfa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="01cfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="01cfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01cfa-111">Permission type</span></span>|<span data-ttu-id="01cfa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01cfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01cfa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01cfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01cfa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01cfa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01cfa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01cfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01cfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01cfa-116">Not supported.</span></span>|
|<span data-ttu-id="01cfa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01cfa-117">Application</span></span>|<span data-ttu-id="01cfa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01cfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01cfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01cfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="01cfa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01cfa-120">Request headers</span></span>
|<span data-ttu-id="01cfa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01cfa-121">Header</span></span>|<span data-ttu-id="01cfa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01cfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01cfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01cfa-123">Authorization</span></span>|<span data-ttu-id="01cfa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01cfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01cfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01cfa-125">Accept</span></span>|<span data-ttu-id="01cfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01cfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01cfa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01cfa-127">Request body</span></span>
<span data-ttu-id="01cfa-128">В тексте запроса укажите представление JSON для объекта enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="01cfa-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="01cfa-129">В следующей таблице показаны свойства, которые необходимы для создания enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="01cfa-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="01cfa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01cfa-130">Property</span></span>|<span data-ttu-id="01cfa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01cfa-131">Type</span></span>|<span data-ttu-id="01cfa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01cfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01cfa-133">id</span><span class="sxs-lookup"><span data-stu-id="01cfa-133">id</span></span>|<span data-ttu-id="01cfa-134">String</span><span class="sxs-lookup"><span data-stu-id="01cfa-134">String</span></span>|<span data-ttu-id="01cfa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01cfa-135">The key of the entity.</span></span>|
|<span data-ttu-id="01cfa-136">content</span><span class="sxs-lookup"><span data-stu-id="01cfa-136">content</span></span>|<span data-ttu-id="01cfa-137">Binary</span><span class="sxs-lookup"><span data-stu-id="01cfa-137">Binary</span></span>|<span data-ttu-id="01cfa-138">Сертификат подписи кода Enterprise Windows в формате необработанные данные.</span><span class="sxs-lookup"><span data-stu-id="01cfa-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="01cfa-139">status</span><span class="sxs-lookup"><span data-stu-id="01cfa-139">status</span></span>|[<span data-ttu-id="01cfa-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="01cfa-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="01cfa-141">Состояние сертификата подготовить к работе или не подготовлен.</span><span class="sxs-lookup"><span data-stu-id="01cfa-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="01cfa-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="01cfa-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="01cfa-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="01cfa-143">subjectName</span></span>|<span data-ttu-id="01cfa-144">String</span><span class="sxs-lookup"><span data-stu-id="01cfa-144">String</span></span>|<span data-ttu-id="01cfa-145">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="01cfa-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="01cfa-146">subject</span><span class="sxs-lookup"><span data-stu-id="01cfa-146">subject</span></span>|<span data-ttu-id="01cfa-147">String</span><span class="sxs-lookup"><span data-stu-id="01cfa-147">String</span></span>|<span data-ttu-id="01cfa-148">Значения субъектов для сертификата.</span><span class="sxs-lookup"><span data-stu-id="01cfa-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="01cfa-149">Имя поставщика</span><span class="sxs-lookup"><span data-stu-id="01cfa-149">issuerName</span></span>|<span data-ttu-id="01cfa-150">String</span><span class="sxs-lookup"><span data-stu-id="01cfa-150">String</span></span>|<span data-ttu-id="01cfa-151">Имя поставщика для сертификата.</span><span class="sxs-lookup"><span data-stu-id="01cfa-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="01cfa-152">издателя</span><span class="sxs-lookup"><span data-stu-id="01cfa-152">issuer</span></span>|<span data-ttu-id="01cfa-153">String</span><span class="sxs-lookup"><span data-stu-id="01cfa-153">String</span></span>|<span data-ttu-id="01cfa-154">Значение издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="01cfa-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="01cfa-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="01cfa-155">expirationDateTime</span></span>|<span data-ttu-id="01cfa-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01cfa-156">DateTimeOffset</span></span>|<span data-ttu-id="01cfa-157">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="01cfa-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="01cfa-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="01cfa-158">uploadDateTime</span></span>|<span data-ttu-id="01cfa-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01cfa-159">DateTimeOffset</span></span>|<span data-ttu-id="01cfa-160">Дата время подписывания кода сертификата при его загрузке.</span><span class="sxs-lookup"><span data-stu-id="01cfa-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="01cfa-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="01cfa-161">Response</span></span>
<span data-ttu-id="01cfa-162">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01cfa-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01cfa-163">Пример</span><span class="sxs-lookup"><span data-stu-id="01cfa-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="01cfa-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="01cfa-164">Request</span></span>
<span data-ttu-id="01cfa-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01cfa-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01cfa-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="01cfa-166">Response</span></span>
<span data-ttu-id="01cfa-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01cfa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




