---
title: Список deviceManagementScriptUserStates
description: Свойства списка и связей объектов deviceManagementScriptUserState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ea4265bced7f323f729de8ea08adf1d0cfc8422
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921502"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="73649-103">Список deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="73649-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="73649-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73649-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73649-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73649-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73649-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73649-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73649-107">Свойства списка и связей объектов [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="73649-107">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73649-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73649-108">Prerequisites</span></span>
<span data-ttu-id="73649-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73649-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73649-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73649-111">Permission type</span></span>|<span data-ttu-id="73649-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73649-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73649-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73649-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73649-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73649-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="73649-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73649-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73649-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73649-116">Not supported.</span></span>|
|<span data-ttu-id="73649-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73649-117">Application</span></span>|<span data-ttu-id="73649-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73649-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73649-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73649-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="73649-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73649-120">Request headers</span></span>
|<span data-ttu-id="73649-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73649-121">Header</span></span>|<span data-ttu-id="73649-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73649-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73649-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73649-123">Authorization</span></span>|<span data-ttu-id="73649-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="73649-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73649-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73649-125">Accept</span></span>|<span data-ttu-id="73649-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73649-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73649-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73649-127">Request body</span></span>
<span data-ttu-id="73649-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73649-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73649-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="73649-129">Response</span></span>
<span data-ttu-id="73649-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73649-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73649-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73649-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="73649-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73649-132">Request</span></span>
<span data-ttu-id="73649-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73649-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="73649-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="73649-134">Response</span></span>
<span data-ttu-id="73649-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="73649-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





