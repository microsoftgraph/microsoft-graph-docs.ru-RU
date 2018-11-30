---
title: Получение windowsManagementAppHealthState
description: Чтение свойства и связи объекта windowsManagementAppHealthState.
ms.openlocfilehash: be59679c926a0500f5b891e63f565fe67419d96d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078776"
---
# <a name="get-windowsmanagementapphealthstate"></a><span data-ttu-id="afac0-103">Получение windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="afac0-103">Get windowsManagementAppHealthState</span></span>

> <span data-ttu-id="afac0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="afac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afac0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afac0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afac0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afac0-107">Чтение свойства и связи объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="afac0-107">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afac0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="afac0-108">Prerequisites</span></span>
<span data-ttu-id="afac0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afac0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afac0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afac0-111">Permission type</span></span>|<span data-ttu-id="afac0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afac0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afac0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afac0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afac0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="afac0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="afac0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afac0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afac0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac0-116">Not supported.</span></span>|
|<span data-ttu-id="afac0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afac0-117">Application</span></span>|<span data-ttu-id="afac0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afac0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afac0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afac0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="afac0-120">Optional query parameters</span></span>
<span data-ttu-id="afac0-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="afac0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="afac0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afac0-122">Request headers</span></span>
|<span data-ttu-id="afac0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afac0-123">Header</span></span>|<span data-ttu-id="afac0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="afac0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afac0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="afac0-125">Authorization</span></span>|<span data-ttu-id="afac0-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="afac0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afac0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="afac0-127">Accept</span></span>|<span data-ttu-id="afac0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="afac0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afac0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afac0-129">Request body</span></span>
<span data-ttu-id="afac0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afac0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afac0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="afac0-131">Response</span></span>
<span data-ttu-id="afac0-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="afac0-132">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afac0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="afac0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="afac0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="afac0-134">Request</span></span>
<span data-ttu-id="afac0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afac0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### <a name="response"></a><span data-ttu-id="afac0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="afac0-136">Response</span></span>
<span data-ttu-id="afac0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="afac0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
    "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
    "healthState": "healthy",
    "installedVersion": "Installed Version value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
    "deviceName": "Device Name value",
    "deviceOSVersion": "Device OSVersion value"
  }
}
```





