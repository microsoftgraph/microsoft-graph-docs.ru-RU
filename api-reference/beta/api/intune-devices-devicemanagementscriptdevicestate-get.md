---
title: Получение deviceManagementScriptDeviceState
description: Чтение свойства и связи объекта deviceManagementScriptDeviceState.
author: tfitzmac
ms.openlocfilehash: 4a050737c4e4aedd9c42228fc685ebfeb3bc02f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349758"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="bccb4-103">Получение deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="bccb4-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="bccb4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bccb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bccb4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bccb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bccb4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bccb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bccb4-107">Чтение свойства и связи объекта [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="bccb4-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bccb4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bccb4-108">Prerequisites</span></span>
<span data-ttu-id="bccb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bccb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bccb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bccb4-111">Permission type</span></span>|<span data-ttu-id="bccb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bccb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bccb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bccb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bccb4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bccb4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bccb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bccb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bccb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bccb4-116">Not supported.</span></span>|
|<span data-ttu-id="bccb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bccb4-117">Application</span></span>|<span data-ttu-id="bccb4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bccb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bccb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bccb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bccb4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bccb4-120">Optional query parameters</span></span>
<span data-ttu-id="bccb4-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bccb4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bccb4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bccb4-122">Request headers</span></span>
|<span data-ttu-id="bccb4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bccb4-123">Header</span></span>|<span data-ttu-id="bccb4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bccb4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bccb4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bccb4-125">Authorization</span></span>|<span data-ttu-id="bccb4-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bccb4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bccb4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bccb4-127">Accept</span></span>|<span data-ttu-id="bccb4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bccb4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bccb4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bccb4-129">Request body</span></span>
<span data-ttu-id="bccb4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bccb4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bccb4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bccb4-131">Response</span></span>
<span data-ttu-id="bccb4-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bccb4-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bccb4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bccb4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bccb4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bccb4-134">Request</span></span>
<span data-ttu-id="bccb4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bccb4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="bccb4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bccb4-136">Response</span></span>
<span data-ttu-id="bccb4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bccb4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
    "runState": "success",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```





