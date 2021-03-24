---
title: Список enterpriseCodeSigningCertificates
description: Список свойств и связей объектов enterpriseCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5ad260b4b36a91f2b78bd60bbc2eae093f39ad8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140835"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="98d55-103">Список enterpriseCodeSigningCertificates</span><span class="sxs-lookup"><span data-stu-id="98d55-103">List enterpriseCodeSigningCertificates</span></span>

<span data-ttu-id="98d55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98d55-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98d55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98d55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98d55-107">Список свойств и связей [объектов enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="98d55-107">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98d55-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98d55-108">Prerequisites</span></span>
<span data-ttu-id="98d55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98d55-111">Permission type</span></span>|<span data-ttu-id="98d55-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98d55-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98d55-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98d55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98d55-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d55-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98d55-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98d55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98d55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d55-116">Not supported.</span></span>|
|<span data-ttu-id="98d55-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98d55-117">Application</span></span>|<span data-ttu-id="98d55-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d55-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98d55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98d55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="98d55-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98d55-120">Request headers</span></span>
|<span data-ttu-id="98d55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98d55-121">Header</span></span>|<span data-ttu-id="98d55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98d55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98d55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d55-123">Authorization</span></span>|<span data-ttu-id="98d55-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98d55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98d55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98d55-125">Accept</span></span>|<span data-ttu-id="98d55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98d55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d55-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98d55-127">Request body</span></span>
<span data-ttu-id="98d55-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98d55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d55-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="98d55-129">Response</span></span>
<span data-ttu-id="98d55-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="98d55-130">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98d55-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98d55-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="98d55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98d55-132">Request</span></span>
<span data-ttu-id="98d55-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98d55-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="98d55-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98d55-134">Response</span></span>
<span data-ttu-id="98d55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98d55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
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
  ]
}
```




