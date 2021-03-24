---
title: Обновление windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f161877e4f4f78479be7cf5aac82ee0f74d340e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133964"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="72242-103">Обновление windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="72242-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="72242-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72242-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72242-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72242-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72242-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72242-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72242-107">Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="72242-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72242-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72242-108">Prerequisites</span></span>
<span data-ttu-id="72242-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72242-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72242-111">Permission type</span></span>|<span data-ttu-id="72242-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72242-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72242-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72242-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72242-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72242-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72242-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72242-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72242-116">Not supported.</span></span>|
|<span data-ttu-id="72242-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="72242-117">Application</span></span>|<span data-ttu-id="72242-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72242-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72242-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72242-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="72242-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72242-120">Request headers</span></span>
|<span data-ttu-id="72242-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72242-121">Header</span></span>|<span data-ttu-id="72242-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72242-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72242-123">Authorization</span></span>|<span data-ttu-id="72242-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72242-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72242-125">Accept</span></span>|<span data-ttu-id="72242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72242-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72242-127">Request body</span></span>
<span data-ttu-id="72242-128">В теле запроса поставляем представление JSON для [объекта windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="72242-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="72242-129">В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="72242-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="72242-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72242-130">Property</span></span>|<span data-ttu-id="72242-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72242-131">Type</span></span>|<span data-ttu-id="72242-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72242-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72242-133">id</span><span class="sxs-lookup"><span data-stu-id="72242-133">id</span></span>|<span data-ttu-id="72242-134">Строка</span><span class="sxs-lookup"><span data-stu-id="72242-134">String</span></span>|<span data-ttu-id="72242-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72242-135">Key of the entity.</span></span>|
|<span data-ttu-id="72242-136">target</span><span class="sxs-lookup"><span data-stu-id="72242-136">target</span></span>|[<span data-ttu-id="72242-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="72242-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="72242-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="72242-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="72242-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="72242-139">Response</span></span>
<span data-ttu-id="72242-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72242-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72242-141">Пример</span><span class="sxs-lookup"><span data-stu-id="72242-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="72242-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="72242-142">Request</span></span>
<span data-ttu-id="72242-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72242-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72242-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="72242-144">Response</span></span>
<span data-ttu-id="72242-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72242-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




