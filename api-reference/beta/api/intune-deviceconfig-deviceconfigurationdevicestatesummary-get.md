---
title: Получение объекта deviceConfigurationDeviceStateSummary
description: Чтение свойств и связей объекта deviceConfigurationDeviceStateSummary.
ms.openlocfilehash: 59e506a288553644616d209ed198ffa1a5a8b714
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079292"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="62d96-103">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="62d96-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="62d96-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62d96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62d96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62d96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62d96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62d96-107">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="62d96-107">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62d96-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="62d96-108">Prerequisites</span></span>
<span data-ttu-id="62d96-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62d96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62d96-111">Permission type</span></span>|<span data-ttu-id="62d96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62d96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62d96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62d96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62d96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="62d96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="62d96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62d96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62d96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d96-116">Not supported.</span></span>|
|<span data-ttu-id="62d96-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62d96-117">Application</span></span>|<span data-ttu-id="62d96-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62d96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62d96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62d96-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62d96-120">Optional query parameters</span></span>
<span data-ttu-id="62d96-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="62d96-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="62d96-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62d96-122">Request headers</span></span>
|<span data-ttu-id="62d96-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62d96-123">Header</span></span>|<span data-ttu-id="62d96-124">Значение</span><span class="sxs-lookup"><span data-stu-id="62d96-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62d96-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="62d96-125">Authorization</span></span>|<span data-ttu-id="62d96-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62d96-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62d96-127">Accept</span><span class="sxs-lookup"><span data-stu-id="62d96-127">Accept</span></span>|<span data-ttu-id="62d96-128">application/json</span><span class="sxs-lookup"><span data-stu-id="62d96-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62d96-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62d96-129">Request body</span></span>
<span data-ttu-id="62d96-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62d96-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62d96-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="62d96-131">Response</span></span>
<span data-ttu-id="62d96-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62d96-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d96-133">Пример</span><span class="sxs-lookup"><span data-stu-id="62d96-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="62d96-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="62d96-134">Request</span></span>
<span data-ttu-id="62d96-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62d96-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="62d96-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="62d96-136">Response</span></span>
<span data-ttu-id="62d96-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="62d96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





