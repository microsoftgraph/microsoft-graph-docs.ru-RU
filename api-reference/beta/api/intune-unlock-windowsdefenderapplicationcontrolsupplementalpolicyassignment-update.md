---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3fc2c4075a30df24507dd7edd095c2cd2755a298
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732130"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="5539d-103">Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="5539d-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="5539d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5539d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5539d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5539d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5539d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5539d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5539d-107">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5539d-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5539d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5539d-108">Prerequisites</span></span>
<span data-ttu-id="5539d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5539d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5539d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5539d-111">Permission type</span></span>|<span data-ttu-id="5539d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5539d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5539d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5539d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5539d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5539d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5539d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5539d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5539d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5539d-116">Not supported.</span></span>|
|<span data-ttu-id="5539d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5539d-117">Application</span></span>|<span data-ttu-id="5539d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5539d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5539d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5539d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5539d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5539d-120">Request headers</span></span>
|<span data-ttu-id="5539d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5539d-121">Header</span></span>|<span data-ttu-id="5539d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5539d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5539d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5539d-123">Authorization</span></span>|<span data-ttu-id="5539d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5539d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5539d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5539d-125">Accept</span></span>|<span data-ttu-id="5539d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5539d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5539d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5539d-127">Request body</span></span>
<span data-ttu-id="5539d-128">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5539d-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="5539d-129">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5539d-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="5539d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5539d-130">Property</span></span>|<span data-ttu-id="5539d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5539d-131">Type</span></span>|<span data-ttu-id="5539d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5539d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5539d-133">id</span><span class="sxs-lookup"><span data-stu-id="5539d-133">id</span></span>|<span data-ttu-id="5539d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5539d-134">String</span></span>|<span data-ttu-id="5539d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5539d-135">Key of the entity.</span></span>|
|<span data-ttu-id="5539d-136">target</span><span class="sxs-lookup"><span data-stu-id="5539d-136">target</span></span>|[<span data-ttu-id="5539d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5539d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5539d-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="5539d-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="5539d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5539d-139">Response</span></span>
<span data-ttu-id="5539d-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5539d-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5539d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5539d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5539d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5539d-142">Request</span></span>
<span data-ttu-id="5539d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5539d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 368

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="5539d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5539d-144">Response</span></span>
<span data-ttu-id="5539d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5539d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





