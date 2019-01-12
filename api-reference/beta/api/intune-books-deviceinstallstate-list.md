---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7622c236a0b2be0703d56c678a07aff570f61cba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919437"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="890be-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="890be-103">List deviceInstallStates</span></span>

> <span data-ttu-id="890be-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="890be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="890be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="890be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="890be-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="890be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="890be-107">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="890be-107">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="890be-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="890be-108">Prerequisites</span></span>
<span data-ttu-id="890be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="890be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="890be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="890be-111">Permission type</span></span>|<span data-ttu-id="890be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="890be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="890be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="890be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="890be-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="890be-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="890be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="890be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="890be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="890be-116">Not supported.</span></span>|
|<span data-ttu-id="890be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="890be-117">Application</span></span>|<span data-ttu-id="890be-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="890be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="890be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="890be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="890be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="890be-120">Request headers</span></span>
|<span data-ttu-id="890be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="890be-121">Header</span></span>|<span data-ttu-id="890be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="890be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="890be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="890be-123">Authorization</span></span>|<span data-ttu-id="890be-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="890be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="890be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="890be-125">Accept</span></span>|<span data-ttu-id="890be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="890be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="890be-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="890be-127">Request body</span></span>
<span data-ttu-id="890be-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="890be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="890be-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="890be-129">Response</span></span>
<span data-ttu-id="890be-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="890be-130">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="890be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="890be-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="890be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="890be-132">Request</span></span>
<span data-ttu-id="890be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="890be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="890be-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="890be-134">Response</span></span>
<span data-ttu-id="890be-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="890be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```





