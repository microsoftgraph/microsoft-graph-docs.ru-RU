---
title: Список Девицеаппманажементтаскс
description: Список свойств и связей объектов Девицеаппманажементтаск.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11b51ca309239c945d948189dec2431ee681e6e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802484"
---
# <a name="list-deviceappmanagementtasks"></a><span data-ttu-id="fc5c2-103">Список Девицеаппманажементтаскс</span><span class="sxs-lookup"><span data-stu-id="fc5c2-103">List deviceAppManagementTasks</span></span>

> <span data-ttu-id="fc5c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc5c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc5c2-106">Список свойств и связей объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="fc5c2-106">List properties and relationships of the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc5c2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc5c2-107">Prerequisites</span></span>
<span data-ttu-id="fc5c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc5c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc5c2-110">Permission type</span></span>|<span data-ttu-id="fc5c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc5c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc5c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc5c2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc5c2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fc5c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc5c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc5c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-115">Not supported.</span></span>|
|<span data-ttu-id="fc5c2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc5c2-116">Application</span></span>|<span data-ttu-id="fc5c2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc5c2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc5c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc5c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="fc5c2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc5c2-119">Request headers</span></span>
|<span data-ttu-id="fc5c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc5c2-120">Header</span></span>|<span data-ttu-id="fc5c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc5c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5c2-122">Authorization</span></span>|<span data-ttu-id="fc5c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc5c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc5c2-124">Accept</span></span>|<span data-ttu-id="fc5c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc5c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc5c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc5c2-126">Request body</span></span>
<span data-ttu-id="fc5c2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc5c2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc5c2-128">Response</span></span>
<span data-ttu-id="fc5c2-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc5c2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fc5c2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc5c2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc5c2-131">Request</span></span>
<span data-ttu-id="fc5c2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="fc5c2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc5c2-133">Response</span></span>
<span data-ttu-id="fc5c2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc5c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




