---
title: Список Виндовсдефендераппликатионконтролсупплементалполициассигнментс
description: Список свойств и связей объектов Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c3fcafa992f0db2576707aab896a8a73db449d4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226701"
---
# <a name="list-windowsdefenderapplicationcontrolsupplementalpolicyassignments"></a><span data-ttu-id="f85c6-103">Список Виндовсдефендераппликатионконтролсупплементалполициассигнментс</span><span class="sxs-lookup"><span data-stu-id="f85c6-103">List windowsDefenderApplicationControlSupplementalPolicyAssignments</span></span>

<span data-ttu-id="f85c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f85c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f85c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f85c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f85c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f85c6-107">Список свойств и связей объектов [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f85c6-107">List properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f85c6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f85c6-108">Prerequisites</span></span>
<span data-ttu-id="f85c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f85c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f85c6-111">Permission type</span></span>|<span data-ttu-id="f85c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f85c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f85c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f85c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f85c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f85c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f85c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f85c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f85c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85c6-116">Not supported.</span></span>|
|<span data-ttu-id="f85c6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f85c6-117">Application</span></span>|<span data-ttu-id="f85c6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f85c6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f85c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f85c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f85c6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f85c6-120">Request headers</span></span>
|<span data-ttu-id="f85c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f85c6-121">Header</span></span>|<span data-ttu-id="f85c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f85c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f85c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f85c6-123">Authorization</span></span>|<span data-ttu-id="f85c6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f85c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f85c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f85c6-125">Accept</span></span>|<span data-ttu-id="f85c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f85c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f85c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f85c6-127">Request body</span></span>
<span data-ttu-id="f85c6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f85c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f85c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85c6-129">Response</span></span>
<span data-ttu-id="f85c6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f85c6-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f85c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f85c6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f85c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f85c6-132">Request</span></span>
<span data-ttu-id="f85c6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f85c6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="f85c6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85c6-134">Response</span></span>
<span data-ttu-id="f85c6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f85c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




