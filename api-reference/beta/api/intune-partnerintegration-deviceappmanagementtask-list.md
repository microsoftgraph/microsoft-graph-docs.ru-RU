---
title: Список Девицеаппманажементтаскс
description: Список свойств и связей объектов Девицеаппманажементтаск.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c80aff6683707db23f34dbbd0115ca4631b041c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461286"
---
# <a name="list-deviceappmanagementtasks"></a><span data-ttu-id="c9cd6-103">Список Девицеаппманажементтаскс</span><span class="sxs-lookup"><span data-stu-id="c9cd6-103">List deviceAppManagementTasks</span></span>

<span data-ttu-id="c9cd6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c9cd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9cd6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9cd6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9cd6-107">Список свойств и связей объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="c9cd6-107">List properties and relationships of the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9cd6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9cd6-108">Prerequisites</span></span>
<span data-ttu-id="c9cd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9cd6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9cd6-111">Permission type</span></span>|<span data-ttu-id="c9cd6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9cd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9cd6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9cd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9cd6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9cd6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c9cd6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9cd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9cd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-116">Not supported.</span></span>|
|<span data-ttu-id="c9cd6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9cd6-117">Application</span></span>|<span data-ttu-id="c9cd6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9cd6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9cd6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9cd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="c9cd6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9cd6-120">Request headers</span></span>
|<span data-ttu-id="c9cd6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9cd6-121">Header</span></span>|<span data-ttu-id="c9cd6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9cd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9cd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9cd6-123">Authorization</span></span>|<span data-ttu-id="c9cd6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9cd6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9cd6-125">Accept</span></span>|<span data-ttu-id="c9cd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9cd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9cd6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9cd6-127">Request body</span></span>
<span data-ttu-id="c9cd6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9cd6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9cd6-129">Response</span></span>
<span data-ttu-id="c9cd6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9cd6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9cd6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9cd6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9cd6-132">Request</span></span>
<span data-ttu-id="c9cd6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="c9cd6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9cd6-134">Response</span></span>
<span data-ttu-id="c9cd6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9cd6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 589

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAppManagementTask",
      "id": "814545cc-45cc-8145-cc45-4581cc454581",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
      "category": "advancedThreatProtection",
      "priority": "high",
      "creator": "Creator value",
      "creatorNotes": "Creator Notes value",
      "assignedTo": "Assigned To value",
      "status": "pending"
    }
  ]
}
```





