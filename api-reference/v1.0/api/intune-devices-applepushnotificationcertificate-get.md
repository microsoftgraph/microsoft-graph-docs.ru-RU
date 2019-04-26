---
title: Получение объекта applePushNotificationCertificate
description: Чтение свойств и связей объекта applePushNotificationCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3bfeb9bb0b0644707121e081cb3c3c78cd858fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566957"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="ee641-103">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ee641-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="ee641-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee641-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee641-105">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ee641-105">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee641-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee641-106">Prerequisites</span></span>
<span data-ttu-id="ee641-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee641-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee641-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee641-109">Permission type</span></span>|<span data-ttu-id="ee641-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee641-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee641-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee641-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee641-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee641-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ee641-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee641-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee641-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee641-114">Not supported.</span></span>|
|<span data-ttu-id="ee641-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee641-115">Application</span></span>|<span data-ttu-id="ee641-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee641-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee641-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee641-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee641-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee641-118">Optional query parameters</span></span>
<span data-ttu-id="ee641-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee641-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee641-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee641-120">Request headers</span></span>
|<span data-ttu-id="ee641-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee641-121">Header</span></span>|<span data-ttu-id="ee641-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee641-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee641-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee641-123">Authorization</span></span>|<span data-ttu-id="ee641-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee641-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee641-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee641-125">Accept</span></span>|<span data-ttu-id="ee641-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee641-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee641-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee641-127">Request body</span></span>
<span data-ttu-id="ee641-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee641-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee641-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee641-129">Response</span></span>
<span data-ttu-id="ee641-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee641-130">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee641-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee641-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee641-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee641-132">Request</span></span>
<span data-ttu-id="ee641-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee641-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="ee641-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee641-134">Response</span></span>
<span data-ttu-id="ee641-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee641-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



