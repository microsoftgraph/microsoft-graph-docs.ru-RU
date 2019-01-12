---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 139b3500c3a1a1d0c79f97ec36005ec0a7fd28ea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911667"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="51141-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="51141-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="51141-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51141-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51141-105">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="51141-105">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51141-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51141-106">Prerequisites</span></span>
<span data-ttu-id="51141-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51141-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51141-109">Permission type</span></span>|<span data-ttu-id="51141-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51141-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51141-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51141-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51141-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51141-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51141-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51141-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51141-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51141-114">Not supported.</span></span>|
|<span data-ttu-id="51141-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51141-115">Application</span></span>|<span data-ttu-id="51141-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51141-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51141-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51141-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51141-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51141-118">Optional query parameters</span></span>
<span data-ttu-id="51141-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51141-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51141-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51141-120">Request headers</span></span>
|<span data-ttu-id="51141-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51141-121">Header</span></span>|<span data-ttu-id="51141-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51141-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51141-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51141-123">Authorization</span></span>|<span data-ttu-id="51141-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51141-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51141-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51141-125">Accept</span></span>|<span data-ttu-id="51141-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51141-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51141-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51141-127">Request body</span></span>
<span data-ttu-id="51141-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51141-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51141-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51141-129">Response</span></span>
<span data-ttu-id="51141-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51141-130">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51141-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51141-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51141-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51141-132">Request</span></span>
<span data-ttu-id="51141-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51141-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="51141-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="51141-134">Response</span></span>
<span data-ttu-id="51141-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51141-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



