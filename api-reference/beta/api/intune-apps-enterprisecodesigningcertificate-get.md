---
title: Получение Ентерприсекодесигнингцертификате
description: Чтение свойств и связей объекта Ентерприсекодесигнингцертификате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7779156aa18f86403a4e4e892da2e618d6e5ec
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974351"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="19e72-103">Получение Ентерприсекодесигнингцертификате</span><span class="sxs-lookup"><span data-stu-id="19e72-103">Get enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="19e72-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19e72-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19e72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19e72-106">Чтение свойств и связей объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="19e72-106">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19e72-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19e72-107">Prerequisites</span></span>
<span data-ttu-id="19e72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19e72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19e72-110">Permission type</span></span>|<span data-ttu-id="19e72-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19e72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19e72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19e72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19e72-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19e72-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19e72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19e72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19e72-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e72-115">Not supported.</span></span>|
|<span data-ttu-id="19e72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19e72-116">Application</span></span>|<span data-ttu-id="19e72-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e72-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19e72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19e72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19e72-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19e72-119">Optional query parameters</span></span>
<span data-ttu-id="19e72-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19e72-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19e72-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19e72-121">Request headers</span></span>
|<span data-ttu-id="19e72-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19e72-122">Header</span></span>|<span data-ttu-id="19e72-123">Значение</span><span class="sxs-lookup"><span data-stu-id="19e72-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19e72-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19e72-124">Authorization</span></span>|<span data-ttu-id="19e72-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19e72-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19e72-126">Accept</span><span class="sxs-lookup"><span data-stu-id="19e72-126">Accept</span></span>|<span data-ttu-id="19e72-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19e72-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19e72-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19e72-128">Request body</span></span>
<span data-ttu-id="19e72-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19e72-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19e72-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="19e72-130">Response</span></span>
<span data-ttu-id="19e72-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19e72-131">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19e72-132">Пример</span><span class="sxs-lookup"><span data-stu-id="19e72-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="19e72-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="19e72-133">Request</span></span>
<span data-ttu-id="19e72-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19e72-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="19e72-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e72-135">Response</span></span>
<span data-ttu-id="19e72-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19e72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




