---
title: Получение deviceManagementScriptAssignment
description: Чтение свойства и связи объекта deviceManagementScriptAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 114f6fa7661f3dadb557af7682a937956444f1a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874776"
---
# <a name="get-devicemanagementscriptassignment"></a><span data-ttu-id="24803-103">Получение deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="24803-103">Get deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="24803-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24803-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24803-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24803-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24803-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="24803-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24803-107">Чтение свойства и связи объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="24803-107">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24803-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24803-108">Prerequisites</span></span>
<span data-ttu-id="24803-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24803-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24803-111">Permission type</span></span>|<span data-ttu-id="24803-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24803-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24803-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24803-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24803-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="24803-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="24803-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24803-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24803-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24803-116">Not supported.</span></span>|
|<span data-ttu-id="24803-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24803-117">Application</span></span>|<span data-ttu-id="24803-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24803-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24803-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24803-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24803-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24803-120">Optional query parameters</span></span>
<span data-ttu-id="24803-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="24803-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24803-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24803-122">Request headers</span></span>
|<span data-ttu-id="24803-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24803-123">Header</span></span>|<span data-ttu-id="24803-124">Значение</span><span class="sxs-lookup"><span data-stu-id="24803-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24803-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="24803-125">Authorization</span></span>|<span data-ttu-id="24803-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="24803-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24803-127">Accept</span><span class="sxs-lookup"><span data-stu-id="24803-127">Accept</span></span>|<span data-ttu-id="24803-128">application/json</span><span class="sxs-lookup"><span data-stu-id="24803-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24803-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24803-129">Request body</span></span>
<span data-ttu-id="24803-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24803-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24803-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="24803-131">Response</span></span>
<span data-ttu-id="24803-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="24803-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24803-133">Пример</span><span class="sxs-lookup"><span data-stu-id="24803-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="24803-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="24803-134">Request</span></span>
<span data-ttu-id="24803-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24803-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="24803-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="24803-136">Response</span></span>
<span data-ttu-id="24803-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="24803-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
    "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





