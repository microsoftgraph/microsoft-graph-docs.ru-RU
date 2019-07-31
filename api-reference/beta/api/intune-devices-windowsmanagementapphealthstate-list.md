---
title: Список Виндовсманажементапфеалсстатес
description: Список свойств и связей объектов Виндовсманажементапфеалсстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59c333d8d6e5d26b4c4a377f6b6ada82d3789d7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981159"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="a3104-103">Список Виндовсманажементапфеалсстатес</span><span class="sxs-lookup"><span data-stu-id="a3104-103">List windowsManagementAppHealthStates</span></span>

> <span data-ttu-id="a3104-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3104-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3104-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3104-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3104-106">Список свойств и связей объектов [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a3104-106">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3104-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3104-107">Prerequisites</span></span>
<span data-ttu-id="a3104-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3104-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3104-110">Permission type</span></span>|<span data-ttu-id="a3104-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3104-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3104-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3104-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3104-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3104-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a3104-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3104-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3104-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3104-115">Not supported.</span></span>|
|<span data-ttu-id="a3104-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3104-116">Application</span></span>|<span data-ttu-id="a3104-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3104-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3104-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3104-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="a3104-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3104-119">Request headers</span></span>
|<span data-ttu-id="a3104-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3104-120">Header</span></span>|<span data-ttu-id="a3104-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3104-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3104-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3104-122">Authorization</span></span>|<span data-ttu-id="a3104-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3104-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3104-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3104-124">Accept</span></span>|<span data-ttu-id="a3104-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3104-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3104-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3104-126">Request body</span></span>
<span data-ttu-id="a3104-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3104-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3104-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3104-128">Response</span></span>
<span data-ttu-id="a3104-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3104-129">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3104-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a3104-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3104-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3104-131">Request</span></span>
<span data-ttu-id="a3104-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3104-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="a3104-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3104-133">Response</span></span>
<span data-ttu-id="a3104-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3104-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
      "healthState": "healthy",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```





