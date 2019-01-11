---
title: Список deviceManagementScriptGroupAssignments
description: Свойства списка и связей объектов deviceManagementScriptGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4773bb8431627f3bb23dc6e1b9584a4c6067de40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816991"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="1b68c-103">Список deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="1b68c-103">List deviceManagementScriptGroupAssignments</span></span>

> <span data-ttu-id="1b68c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b68c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b68c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b68c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b68c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b68c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b68c-107">Свойства списка и связей объектов [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1b68c-107">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b68c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b68c-108">Prerequisites</span></span>
<span data-ttu-id="1b68c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b68c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b68c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b68c-111">Permission type</span></span>|<span data-ttu-id="1b68c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b68c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b68c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b68c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b68c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b68c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1b68c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b68c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b68c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b68c-116">Not supported.</span></span>|
|<span data-ttu-id="1b68c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b68c-117">Application</span></span>|<span data-ttu-id="1b68c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b68c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b68c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b68c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="1b68c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b68c-120">Request headers</span></span>
|<span data-ttu-id="1b68c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b68c-121">Header</span></span>|<span data-ttu-id="1b68c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b68c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b68c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b68c-123">Authorization</span></span>|<span data-ttu-id="1b68c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b68c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b68c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b68c-125">Accept</span></span>|<span data-ttu-id="1b68c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b68c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b68c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b68c-127">Request body</span></span>
<span data-ttu-id="1b68c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b68c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b68c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b68c-129">Response</span></span>
<span data-ttu-id="1b68c-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b68c-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b68c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1b68c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b68c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b68c-132">Request</span></span>
<span data-ttu-id="1b68c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b68c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="1b68c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b68c-134">Response</span></span>
<span data-ttu-id="1b68c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b68c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```





