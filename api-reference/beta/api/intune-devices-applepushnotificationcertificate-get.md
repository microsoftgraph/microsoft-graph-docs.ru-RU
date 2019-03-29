---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfaba72d0c4c779026ec17f299caffbb7aa301dd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969129"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="f10ef-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f10ef-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="f10ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f10ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f10ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10ef-106">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="f10ef-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f10ef-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f10ef-107">Prerequisites</span></span>
<span data-ttu-id="f10ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f10ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f10ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f10ef-110">Permission type</span></span>|<span data-ttu-id="f10ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f10ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f10ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f10ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f10ef-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f10ef-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f10ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f10ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f10ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10ef-115">Not supported.</span></span>|
|<span data-ttu-id="f10ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f10ef-116">Application</span></span>|<span data-ttu-id="f10ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f10ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f10ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f10ef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f10ef-119">Optional query parameters</span></span>
<span data-ttu-id="f10ef-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f10ef-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f10ef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f10ef-121">Request headers</span></span>
|<span data-ttu-id="f10ef-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f10ef-122">Header</span></span>|<span data-ttu-id="f10ef-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f10ef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f10ef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f10ef-124">Authorization</span></span>|<span data-ttu-id="f10ef-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f10ef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f10ef-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f10ef-126">Accept</span></span>|<span data-ttu-id="f10ef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f10ef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10ef-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f10ef-128">Request body</span></span>
<span data-ttu-id="f10ef-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f10ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f10ef-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f10ef-130">Response</span></span>
<span data-ttu-id="f10ef-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f10ef-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f10ef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f10ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f10ef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f10ef-133">Request</span></span>
<span data-ttu-id="f10ef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f10ef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="f10ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f10ef-135">Response</span></span>
<span data-ttu-id="f10ef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f10ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




