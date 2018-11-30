---
title: Список deviceManagementScriptAssignments
description: Свойства списка и связей объектов deviceManagementScriptAssignment.
ms.openlocfilehash: 2cb42c62ea2e0c623dcb91c0e367ea5d79bd19b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078286"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="4da65-103">Список deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="4da65-103">List deviceManagementScriptAssignments</span></span>

> <span data-ttu-id="4da65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4da65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4da65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4da65-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4da65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4da65-107">Свойства списка и связей объектов [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4da65-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4da65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4da65-108">Prerequisites</span></span>
<span data-ttu-id="4da65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4da65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da65-111">Permission type</span></span>|<span data-ttu-id="4da65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4da65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4da65-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4da65-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4da65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4da65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da65-116">Not supported.</span></span>|
|<span data-ttu-id="4da65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4da65-117">Application</span></span>|<span data-ttu-id="4da65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4da65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4da65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4da65-120">Request headers</span></span>
|<span data-ttu-id="4da65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4da65-121">Header</span></span>|<span data-ttu-id="4da65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4da65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4da65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4da65-123">Authorization</span></span>|<span data-ttu-id="4da65-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4da65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4da65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4da65-125">Accept</span></span>|<span data-ttu-id="4da65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4da65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4da65-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4da65-127">Request body</span></span>
<span data-ttu-id="4da65-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4da65-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4da65-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4da65-129">Response</span></span>
<span data-ttu-id="4da65-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4da65-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4da65-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4da65-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4da65-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4da65-132">Request</span></span>
<span data-ttu-id="4da65-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4da65-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="4da65-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4da65-134">Response</span></span>
<span data-ttu-id="4da65-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4da65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





