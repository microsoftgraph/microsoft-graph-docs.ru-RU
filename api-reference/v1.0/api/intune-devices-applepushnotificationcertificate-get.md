---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
ms.openlocfilehash: eabab534b812cd35eb4652c530b08120b699c330
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026418"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="d4077-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d4077-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="d4077-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4077-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4077-105">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d4077-105">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4077-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d4077-106">Prerequisites</span></span>
<span data-ttu-id="d4077-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4077-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4077-109">Permission type</span></span>|<span data-ttu-id="d4077-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4077-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4077-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4077-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4077-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4077-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d4077-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4077-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4077-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4077-114">Not supported.</span></span>|
|<span data-ttu-id="d4077-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4077-115">Application</span></span>|<span data-ttu-id="d4077-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4077-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4077-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4077-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4077-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4077-118">Optional query parameters</span></span>
<span data-ttu-id="d4077-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d4077-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4077-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4077-120">Request headers</span></span>
|<span data-ttu-id="d4077-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4077-121">Header</span></span>|<span data-ttu-id="d4077-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4077-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4077-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4077-123">Authorization</span></span>|<span data-ttu-id="d4077-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d4077-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4077-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4077-125">Accept</span></span>|<span data-ttu-id="d4077-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4077-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4077-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4077-127">Request body</span></span>
<span data-ttu-id="d4077-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4077-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4077-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4077-129">Response</span></span>
<span data-ttu-id="d4077-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4077-130">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4077-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d4077-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4077-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4077-132">Request</span></span>
<span data-ttu-id="d4077-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4077-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="d4077-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4077-134">Response</span></span>
<span data-ttu-id="d4077-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d4077-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Certificate value"
  }
}
```



