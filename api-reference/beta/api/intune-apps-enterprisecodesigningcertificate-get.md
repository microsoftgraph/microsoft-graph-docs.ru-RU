---
title: Получение enterpriseCodeSigningCertificate
description: Чтение свойства и связи объекта enterpriseCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c1d280b44e583d9218be1128c1683c1db0c91680
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874811"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="45025-103">Получение enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="45025-103">Get enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="45025-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45025-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45025-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45025-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45025-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45025-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45025-107">Чтение свойства и связи объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="45025-107">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45025-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45025-108">Prerequisites</span></span>
<span data-ttu-id="45025-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45025-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45025-111">Permission type</span></span>|<span data-ttu-id="45025-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45025-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45025-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45025-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45025-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45025-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45025-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45025-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45025-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45025-116">Not supported.</span></span>|
|<span data-ttu-id="45025-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45025-117">Application</span></span>|<span data-ttu-id="45025-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45025-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45025-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45025-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45025-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45025-120">Optional query parameters</span></span>
<span data-ttu-id="45025-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45025-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45025-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45025-122">Request headers</span></span>
|<span data-ttu-id="45025-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45025-123">Header</span></span>|<span data-ttu-id="45025-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45025-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45025-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="45025-125">Authorization</span></span>|<span data-ttu-id="45025-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45025-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45025-127">Accept</span><span class="sxs-lookup"><span data-stu-id="45025-127">Accept</span></span>|<span data-ttu-id="45025-128">application/json</span><span class="sxs-lookup"><span data-stu-id="45025-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45025-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45025-129">Request body</span></span>
<span data-ttu-id="45025-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45025-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45025-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="45025-131">Response</span></span>
<span data-ttu-id="45025-132">Успешно завершена, этот метод возвращает `200 OK` объект [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45025-132">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45025-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45025-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="45025-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45025-134">Request</span></span>
<span data-ttu-id="45025-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45025-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="45025-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45025-136">Response</span></span>
<span data-ttu-id="45025-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45025-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "value": {
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
}
```





