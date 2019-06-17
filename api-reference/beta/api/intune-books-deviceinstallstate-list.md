---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49a2667375c30093f0ad0309a79e3bac2ef8efbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972496"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="45a28-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="45a28-103">List deviceInstallStates</span></span>

> <span data-ttu-id="45a28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45a28-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45a28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a28-106">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="45a28-106">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a28-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45a28-107">Prerequisites</span></span>
<span data-ttu-id="45a28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45a28-110">Permission type</span></span>|<span data-ttu-id="45a28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45a28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45a28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45a28-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45a28-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45a28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45a28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a28-115">Not supported.</span></span>|
|<span data-ttu-id="45a28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45a28-116">Application</span></span>|<span data-ttu-id="45a28-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45a28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="45a28-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45a28-119">Request headers</span></span>
|<span data-ttu-id="45a28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45a28-120">Header</span></span>|<span data-ttu-id="45a28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45a28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a28-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45a28-122">Authorization</span></span>|<span data-ttu-id="45a28-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45a28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a28-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45a28-124">Accept</span></span>|<span data-ttu-id="45a28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45a28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a28-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45a28-126">Request body</span></span>
<span data-ttu-id="45a28-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45a28-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a28-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="45a28-128">Response</span></span>
<span data-ttu-id="45a28-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45a28-129">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a28-130">Пример</span><span class="sxs-lookup"><span data-stu-id="45a28-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a28-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45a28-131">Request</span></span>
<span data-ttu-id="45a28-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45a28-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="45a28-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="45a28-133">Response</span></span>
<span data-ttu-id="45a28-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45a28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





