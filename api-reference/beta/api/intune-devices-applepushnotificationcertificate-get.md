---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: tfitzmac
ms.openlocfilehash: 0b7cf69922386b6b025bf23b4ddbcfeefc67bbb8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357724"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="d8a6b-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d8a6b-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="d8a6b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a6b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8a6b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8a6b-107">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d8a6b-107">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8a6b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8a6b-108">Prerequisites</span></span>
<span data-ttu-id="d8a6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8a6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8a6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a6b-111">Permission type</span></span>|<span data-ttu-id="d8a6b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8a6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8a6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8a6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8a6b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8a6b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8a6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8a6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8a6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-116">Not supported.</span></span>|
|<span data-ttu-id="d8a6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8a6b-117">Application</span></span>|<span data-ttu-id="d8a6b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8a6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8a6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8a6b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8a6b-120">Optional query parameters</span></span>
<span data-ttu-id="d8a6b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8a6b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8a6b-122">Request headers</span></span>
|<span data-ttu-id="d8a6b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8a6b-123">Header</span></span>|<span data-ttu-id="d8a6b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a6b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8a6b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8a6b-125">Authorization</span></span>|<span data-ttu-id="d8a6b-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8a6b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8a6b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d8a6b-127">Accept</span></span>|<span data-ttu-id="d8a6b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8a6b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8a6b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8a6b-129">Request body</span></span>
<span data-ttu-id="d8a6b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8a6b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8a6b-131">Response</span></span>
<span data-ttu-id="d8a6b-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-132">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8a6b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d8a6b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8a6b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8a6b-134">Request</span></span>
<span data-ttu-id="d8a6b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="d8a6b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8a6b-136">Response</span></span>
<span data-ttu-id="d8a6b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8a6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateUploadStatus": "Certificate Upload Status value",
    "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
    "certificate": "Certificate value"
  }
}
```





