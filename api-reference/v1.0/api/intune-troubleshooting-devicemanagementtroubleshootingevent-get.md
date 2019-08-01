---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a2de223a416964cb4562fae9ec3851ea8fe24c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025696"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="e48d6-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e48d6-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="e48d6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e48d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e48d6-105">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e48d6-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e48d6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e48d6-106">Prerequisites</span></span>
<span data-ttu-id="e48d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e48d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e48d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e48d6-109">Permission type</span></span>|<span data-ttu-id="e48d6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e48d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e48d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e48d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e48d6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e48d6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e48d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e48d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e48d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e48d6-114">Not supported.</span></span>|
|<span data-ttu-id="e48d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e48d6-115">Application</span></span>|<span data-ttu-id="e48d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e48d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e48d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e48d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e48d6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e48d6-118">Optional query parameters</span></span>
<span data-ttu-id="e48d6-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e48d6-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e48d6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e48d6-120">Request headers</span></span>
|<span data-ttu-id="e48d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e48d6-121">Header</span></span>|<span data-ttu-id="e48d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e48d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e48d6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e48d6-123">Authorization</span></span>|<span data-ttu-id="e48d6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e48d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e48d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e48d6-125">Accept</span></span>|<span data-ttu-id="e48d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e48d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e48d6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e48d6-127">Request body</span></span>
<span data-ttu-id="e48d6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e48d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e48d6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e48d6-129">Response</span></span>
<span data-ttu-id="e48d6-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e48d6-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e48d6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e48d6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e48d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e48d6-132">Request</span></span>
<span data-ttu-id="e48d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e48d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e48d6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e48d6-134">Response</span></span>
<span data-ttu-id="e48d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e48d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```



