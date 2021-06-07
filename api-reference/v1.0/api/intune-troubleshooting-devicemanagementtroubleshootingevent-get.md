---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4df24a618f71804090b1b4ad5cd8b1c320664be
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732943"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="2c3d3-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="2c3d3-103">Get deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="2c3d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c3d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c3d3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c3d3-106">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="2c3d3-106">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c3d3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2c3d3-107">Prerequisites</span></span>
<span data-ttu-id="2c3d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c3d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c3d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c3d3-110">Permission type</span></span>|<span data-ttu-id="2c3d3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c3d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c3d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c3d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c3d3-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c3d3-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2c3d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c3d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c3d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-115">Not supported.</span></span>|
|<span data-ttu-id="2c3d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c3d3-116">Application</span></span>|<span data-ttu-id="2c3d3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c3d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c3d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c3d3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c3d3-119">Optional query parameters</span></span>
<span data-ttu-id="2c3d3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c3d3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c3d3-121">Request headers</span></span>
|<span data-ttu-id="2c3d3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c3d3-122">Header</span></span>|<span data-ttu-id="2c3d3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2c3d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c3d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c3d3-124">Authorization</span></span>|<span data-ttu-id="2c3d3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c3d3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2c3d3-126">Accept</span></span>|<span data-ttu-id="2c3d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c3d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c3d3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c3d3-128">Request body</span></span>
<span data-ttu-id="2c3d3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c3d3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c3d3-130">Response</span></span>
<span data-ttu-id="2c3d3-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-131">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c3d3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2c3d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c3d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c3d3-133">Request</span></span>
<span data-ttu-id="2c3d3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="2c3d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c3d3-135">Response</span></span>
<span data-ttu-id="2c3d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c3d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









