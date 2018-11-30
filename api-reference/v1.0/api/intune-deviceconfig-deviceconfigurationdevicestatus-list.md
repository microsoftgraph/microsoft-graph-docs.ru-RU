---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
ms.openlocfilehash: 5914c6a63a533c9c659f44072b21dd5f0b99c579
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026880"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="3c7c5-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="3c7c5-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="3c7c5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c7c5-105">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="3c7c5-105">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c7c5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3c7c5-106">Prerequisites</span></span>
<span data-ttu-id="3c7c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c7c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c7c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c7c5-109">Permission type</span></span>|<span data-ttu-id="3c7c5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c7c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c7c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c7c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c7c5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c7c5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c7c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c7c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c7c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-114">Not supported.</span></span>|
|<span data-ttu-id="3c7c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c7c5-115">Application</span></span>|<span data-ttu-id="3c7c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c7c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c7c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3c7c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c7c5-118">Request headers</span></span>
|<span data-ttu-id="3c7c5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c7c5-119">Header</span></span>|<span data-ttu-id="3c7c5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3c7c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c7c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c7c5-121">Authorization</span></span>|<span data-ttu-id="3c7c5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c7c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c7c5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3c7c5-123">Accept</span></span>|<span data-ttu-id="3c7c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c7c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c7c5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c7c5-125">Request body</span></span>
<span data-ttu-id="3c7c5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c7c5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c7c5-127">Response</span></span>
<span data-ttu-id="3c7c5-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c7c5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3c7c5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c7c5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c7c5-130">Request</span></span>
<span data-ttu-id="3c7c5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c7c5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="3c7c5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c7c5-132">Response</span></span>
<span data-ttu-id="3c7c5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3c7c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



