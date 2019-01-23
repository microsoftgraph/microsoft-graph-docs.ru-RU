---
title: Список enterpriseCodeSigningCertificates
description: Свойства списка и связей объектов enterpriseCodeSigningCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 354ad56cd01a89a4fe5d3050096671217d24295e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394903"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="d3acb-103">Список enterpriseCodeSigningCertificates</span><span class="sxs-lookup"><span data-stu-id="d3acb-103">List enterpriseCodeSigningCertificates</span></span>

> <span data-ttu-id="d3acb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d3acb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3acb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3acb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3acb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3acb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3acb-107">Свойства списка и связей объектов [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d3acb-107">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3acb-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d3acb-108">Prerequisites</span></span>
<span data-ttu-id="d3acb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3acb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d3acb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3acb-111">Permission type</span></span>|<span data-ttu-id="d3acb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3acb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3acb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3acb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3acb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3acb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3acb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3acb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3acb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3acb-116">Not supported.</span></span>|
|<span data-ttu-id="d3acb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3acb-117">Application</span></span>|<span data-ttu-id="d3acb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3acb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3acb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3acb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="d3acb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3acb-120">Request headers</span></span>
|<span data-ttu-id="d3acb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3acb-121">Header</span></span>|<span data-ttu-id="d3acb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3acb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3acb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3acb-123">Authorization</span></span>|<span data-ttu-id="d3acb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d3acb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3acb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3acb-125">Accept</span></span>|<span data-ttu-id="d3acb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3acb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3acb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3acb-127">Request body</span></span>
<span data-ttu-id="d3acb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3acb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3acb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3acb-129">Response</span></span>
<span data-ttu-id="d3acb-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d3acb-130">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3acb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3acb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3acb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3acb-132">Request</span></span>
<span data-ttu-id="d3acb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3acb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="d3acb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3acb-134">Response</span></span>
<span data-ttu-id="d3acb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d3acb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




