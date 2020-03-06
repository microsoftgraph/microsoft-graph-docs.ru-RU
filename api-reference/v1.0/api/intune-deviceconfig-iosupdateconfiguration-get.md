---
title: Get iosUpdateConfiguration
description: Чтение свойств и связей объекта iosUpdateConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43ea7e707de03fba172fc4d3a883bb3cd16f6f29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514489"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="0b2a9-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b2a9-103">Get iosUpdateConfiguration</span></span>

<span data-ttu-id="0b2a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b2a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b2a9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b2a9-106">Чтение свойств и связей объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b2a9-106">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b2a9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0b2a9-107">Prerequisites</span></span>
<span data-ttu-id="0b2a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b2a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b2a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b2a9-110">Permission type</span></span>|<span data-ttu-id="0b2a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b2a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b2a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b2a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b2a9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b2a9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b2a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b2a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b2a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-115">Not supported.</span></span>|
|<span data-ttu-id="0b2a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b2a9-116">Application</span></span>|<span data-ttu-id="0b2a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b2a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b2a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b2a9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b2a9-119">Optional query parameters</span></span>
<span data-ttu-id="0b2a9-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b2a9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b2a9-121">Request headers</span></span>
|<span data-ttu-id="0b2a9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b2a9-122">Header</span></span>|<span data-ttu-id="0b2a9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0b2a9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b2a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b2a9-124">Authorization</span></span>|<span data-ttu-id="0b2a9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b2a9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0b2a9-126">Accept</span></span>|<span data-ttu-id="0b2a9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0b2a9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b2a9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b2a9-128">Request body</span></span>
<span data-ttu-id="0b2a9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b2a9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b2a9-130">Response</span></span>
<span data-ttu-id="0b2a9-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-131">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b2a9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0b2a9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b2a9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b2a9-133">Request</span></span>
<span data-ttu-id="0b2a9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0b2a9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b2a9-135">Response</span></span>
<span data-ttu-id="0b2a9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b2a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```




