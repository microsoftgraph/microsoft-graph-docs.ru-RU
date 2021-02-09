---
title: Перечисление объектов managedDevice
description: Перечисление свойств и связей объектов managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35b96d57793a3068f9564639d39e6f3cd681e2b8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160586"
---
# <a name="list-manageddevices"></a><span data-ttu-id="dbec9-103">Перечисление объектов managedDevice</span><span class="sxs-lookup"><span data-stu-id="dbec9-103">List managedDevices</span></span>

<span data-ttu-id="dbec9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbec9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbec9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbec9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbec9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbec9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbec9-107">Перечисление свойств и связей объектов [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="dbec9-107">List properties and relationships of the [managedDevice](../resources/intune-shared-manageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbec9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dbec9-108">Prerequisites</span></span>
<span data-ttu-id="dbec9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbec9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbec9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbec9-111">Permission type</span></span>|<span data-ttu-id="dbec9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbec9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbec9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbec9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbec9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbec9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbec9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbec9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbec9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbec9-116">Not supported.</span></span>|
|<span data-ttu-id="dbec9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbec9-117">Application</span></span>|<span data-ttu-id="dbec9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbec9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbec9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbec9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="dbec9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dbec9-120">Request headers</span></span>
|<span data-ttu-id="dbec9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbec9-121">Header</span></span>|<span data-ttu-id="dbec9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dbec9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbec9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbec9-123">Authorization</span></span>|<span data-ttu-id="dbec9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbec9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbec9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dbec9-125">Accept</span></span>|<span data-ttu-id="dbec9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbec9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbec9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbec9-127">Request body</span></span>
<span data-ttu-id="dbec9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbec9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbec9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbec9-129">Response</span></span>
<span data-ttu-id="dbec9-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDevice](../resources/intune-shared-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbec9-130">If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/intune-shared-manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbec9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dbec9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbec9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbec9-132">Request</span></span>
<span data-ttu-id="dbec9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbec9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices
```

### <a name="response"></a><span data-ttu-id="dbec9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbec9-134">Response</span></span>
<span data-ttu-id="dbec9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbec9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 145

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70"
    }
  ]
}
```




