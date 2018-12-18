---
title: Получение объекта deviceConfigurationDeviceStateSummary
description: Чтение свойств и связей объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
ms.openlocfilehash: 580fa843641ca164ac7af0fa5cbf536cd23cb422
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322003"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="35079-103">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="35079-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="35079-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35079-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35079-105">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="35079-105">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35079-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="35079-106">Prerequisites</span></span>
<span data-ttu-id="35079-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35079-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35079-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35079-109">Permission type</span></span>|<span data-ttu-id="35079-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35079-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35079-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35079-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35079-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35079-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35079-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35079-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35079-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35079-114">Not supported.</span></span>|
|<span data-ttu-id="35079-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35079-115">Application</span></span>|<span data-ttu-id="35079-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35079-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35079-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35079-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35079-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35079-118">Optional query parameters</span></span>
<span data-ttu-id="35079-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35079-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35079-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35079-120">Request headers</span></span>
|<span data-ttu-id="35079-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35079-121">Header</span></span>|<span data-ttu-id="35079-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35079-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35079-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35079-123">Authorization</span></span>|<span data-ttu-id="35079-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35079-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35079-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35079-125">Accept</span></span>|<span data-ttu-id="35079-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35079-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35079-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35079-127">Request body</span></span>
<span data-ttu-id="35079-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35079-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35079-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="35079-129">Response</span></span>
<span data-ttu-id="35079-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35079-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35079-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35079-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="35079-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35079-132">Request</span></span>
<span data-ttu-id="35079-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35079-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="35079-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="35079-134">Response</span></span>
<span data-ttu-id="35079-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35079-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```



