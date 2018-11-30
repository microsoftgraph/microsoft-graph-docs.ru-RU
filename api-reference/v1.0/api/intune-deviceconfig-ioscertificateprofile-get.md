---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
ms.openlocfilehash: fb0cbb214f79c5621c093da9dff4b82ad9021f46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026455"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="9de5b-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9de5b-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="9de5b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9de5b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9de5b-105">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9de5b-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9de5b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9de5b-106">Prerequisites</span></span>
<span data-ttu-id="9de5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9de5b-109">Permission type</span></span>|<span data-ttu-id="9de5b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9de5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9de5b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9de5b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9de5b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9de5b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9de5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9de5b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9de5b-114">Not supported.</span></span>|
|<span data-ttu-id="9de5b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9de5b-115">Application</span></span>|<span data-ttu-id="9de5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9de5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9de5b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9de5b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9de5b-118">Optional query parameters</span></span>
<span data-ttu-id="9de5b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9de5b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9de5b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9de5b-120">Request headers</span></span>
|<span data-ttu-id="9de5b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9de5b-121">Header</span></span>|<span data-ttu-id="9de5b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9de5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9de5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9de5b-123">Authorization</span></span>|<span data-ttu-id="9de5b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9de5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9de5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9de5b-125">Accept</span></span>|<span data-ttu-id="9de5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9de5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9de5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9de5b-127">Request body</span></span>
<span data-ttu-id="9de5b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9de5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9de5b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9de5b-129">Response</span></span>
<span data-ttu-id="9de5b-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9de5b-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de5b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9de5b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9de5b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9de5b-132">Request</span></span>
<span data-ttu-id="9de5b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9de5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9de5b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9de5b-134">Response</span></span>
<span data-ttu-id="9de5b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9de5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



