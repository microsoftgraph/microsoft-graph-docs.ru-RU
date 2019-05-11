---
title: Получение Виндовсманажементапфеалсстате
description: Чтение свойств и связей объекта Виндовсманажементапфеалсстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fc79ccd4e2376121a8cf6e8459c99a37d5c1016
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909038"
---
# <a name="get-windowsmanagementapphealthstate"></a><span data-ttu-id="d6bbe-103">Получение Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="d6bbe-103">Get windowsManagementAppHealthState</span></span>

> <span data-ttu-id="d6bbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bbe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bbe-106">Чтение свойств и связей объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d6bbe-106">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6bbe-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6bbe-107">Prerequisites</span></span>
<span data-ttu-id="d6bbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6bbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6bbe-110">Permission type</span></span>|<span data-ttu-id="d6bbe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6bbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6bbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6bbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6bbe-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6bbe-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6bbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6bbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6bbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-115">Not supported.</span></span>|
|<span data-ttu-id="d6bbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6bbe-116">Application</span></span>|<span data-ttu-id="d6bbe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6bbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6bbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6bbe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6bbe-119">Optional query parameters</span></span>
<span data-ttu-id="d6bbe-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6bbe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6bbe-121">Request headers</span></span>
|<span data-ttu-id="d6bbe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6bbe-122">Header</span></span>|<span data-ttu-id="d6bbe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d6bbe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6bbe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6bbe-124">Authorization</span></span>|<span data-ttu-id="d6bbe-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6bbe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d6bbe-126">Accept</span></span>|<span data-ttu-id="d6bbe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6bbe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6bbe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6bbe-128">Request body</span></span>
<span data-ttu-id="d6bbe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6bbe-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6bbe-130">Response</span></span>
<span data-ttu-id="d6bbe-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-131">If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6bbe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d6bbe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6bbe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6bbe-133">Request</span></span>
<span data-ttu-id="d6bbe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### <a name="response"></a><span data-ttu-id="d6bbe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6bbe-135">Response</span></span>
<span data-ttu-id="d6bbe-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6bbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




