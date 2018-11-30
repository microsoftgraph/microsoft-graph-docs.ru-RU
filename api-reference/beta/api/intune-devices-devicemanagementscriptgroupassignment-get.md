---
title: Получение deviceManagementScriptGroupAssignment
description: Чтение свойства и связи объекта deviceManagementScriptGroupAssignment.
ms.openlocfilehash: ca37bb26c46cf7a5195b393395fe8fee96fd405b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081074"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="45140-103">Получение deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="45140-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="45140-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45140-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45140-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45140-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45140-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45140-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45140-107">Чтение свойства и связи объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="45140-107">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45140-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45140-108">Prerequisites</span></span>
<span data-ttu-id="45140-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45140-111">Permission type</span></span>|<span data-ttu-id="45140-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45140-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45140-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45140-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45140-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45140-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45140-116">Not supported.</span></span>|
|<span data-ttu-id="45140-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45140-117">Application</span></span>|<span data-ttu-id="45140-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45140-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45140-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45140-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45140-120">Optional query parameters</span></span>
<span data-ttu-id="45140-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45140-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45140-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45140-122">Request headers</span></span>
|<span data-ttu-id="45140-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45140-123">Header</span></span>|<span data-ttu-id="45140-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45140-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45140-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="45140-125">Authorization</span></span>|<span data-ttu-id="45140-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45140-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45140-127">Accept</span><span class="sxs-lookup"><span data-stu-id="45140-127">Accept</span></span>|<span data-ttu-id="45140-128">application/json</span><span class="sxs-lookup"><span data-stu-id="45140-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45140-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45140-129">Request body</span></span>
<span data-ttu-id="45140-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45140-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45140-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="45140-131">Response</span></span>
<span data-ttu-id="45140-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45140-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45140-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45140-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="45140-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45140-134">Request</span></span>
<span data-ttu-id="45140-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45140-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="45140-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45140-136">Response</span></span>
<span data-ttu-id="45140-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="45140-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```





