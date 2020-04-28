---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 923d4dd424b25a58380af2f369c0b79d2b524727
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450182"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="5c85e-103">Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="5c85e-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="5c85e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c85e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c85e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c85e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c85e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c85e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c85e-107">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c85e-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c85e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c85e-108">Prerequisites</span></span>
<span data-ttu-id="5c85e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c85e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c85e-111">Permission type</span></span>|<span data-ttu-id="5c85e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c85e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c85e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c85e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c85e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c85e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c85e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c85e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c85e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c85e-116">Not supported.</span></span>|
|<span data-ttu-id="5c85e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c85e-117">Application</span></span>|<span data-ttu-id="5c85e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c85e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c85e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c85e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5c85e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c85e-120">Request headers</span></span>
|<span data-ttu-id="5c85e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c85e-121">Header</span></span>|<span data-ttu-id="5c85e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5c85e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c85e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c85e-123">Authorization</span></span>|<span data-ttu-id="5c85e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c85e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c85e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c85e-125">Accept</span></span>|<span data-ttu-id="5c85e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c85e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c85e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c85e-127">Request body</span></span>
<span data-ttu-id="5c85e-128">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c85e-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="5c85e-129">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c85e-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="5c85e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c85e-130">Property</span></span>|<span data-ttu-id="5c85e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5c85e-131">Type</span></span>|<span data-ttu-id="5c85e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5c85e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c85e-133">id</span><span class="sxs-lookup"><span data-stu-id="5c85e-133">id</span></span>|<span data-ttu-id="5c85e-134">String</span><span class="sxs-lookup"><span data-stu-id="5c85e-134">String</span></span>|<span data-ttu-id="5c85e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c85e-135">Key of the entity.</span></span>|
|<span data-ttu-id="5c85e-136">target</span><span class="sxs-lookup"><span data-stu-id="5c85e-136">target</span></span>|[<span data-ttu-id="5c85e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c85e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c85e-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="5c85e-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="5c85e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c85e-139">Response</span></span>
<span data-ttu-id="5c85e-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c85e-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c85e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5c85e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c85e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c85e-142">Request</span></span>
<span data-ttu-id="5c85e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c85e-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5c85e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c85e-144">Response</span></span>
<span data-ttu-id="5c85e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c85e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



