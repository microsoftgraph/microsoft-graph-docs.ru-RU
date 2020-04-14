---
title: Создание Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 008bc6715ef60d21e468a8078d67076c91e66c6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457237"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="01f3b-103">Создание Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="01f3b-103">Create windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="01f3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01f3b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01f3b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01f3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01f3b-107">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="01f3b-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01f3b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01f3b-108">Prerequisites</span></span>
<span data-ttu-id="01f3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f3b-111">Permission type</span></span>|<span data-ttu-id="01f3b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01f3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01f3b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f3b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01f3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01f3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f3b-116">Not supported.</span></span>|
|<span data-ttu-id="01f3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01f3b-117">Application</span></span>|<span data-ttu-id="01f3b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f3b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01f3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="01f3b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01f3b-120">Request headers</span></span>
|<span data-ttu-id="01f3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01f3b-121">Header</span></span>|<span data-ttu-id="01f3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01f3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01f3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f3b-123">Authorization</span></span>|<span data-ttu-id="01f3b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01f3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01f3b-125">Accept</span></span>|<span data-ttu-id="01f3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01f3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f3b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01f3b-127">Request body</span></span>
<span data-ttu-id="01f3b-128">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01f3b-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyAssignment object.</span></span>

<span data-ttu-id="01f3b-129">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполициассигнмент.</span><span class="sxs-lookup"><span data-stu-id="01f3b-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyAssignment.</span></span>

|<span data-ttu-id="01f3b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01f3b-130">Property</span></span>|<span data-ttu-id="01f3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01f3b-131">Type</span></span>|<span data-ttu-id="01f3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01f3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f3b-133">id</span><span class="sxs-lookup"><span data-stu-id="01f3b-133">id</span></span>|<span data-ttu-id="01f3b-134">String</span><span class="sxs-lookup"><span data-stu-id="01f3b-134">String</span></span>|<span data-ttu-id="01f3b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01f3b-135">Key of the entity.</span></span>|
|<span data-ttu-id="01f3b-136">target</span><span class="sxs-lookup"><span data-stu-id="01f3b-136">target</span></span>|[<span data-ttu-id="01f3b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="01f3b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="01f3b-138">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="01f3b-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="01f3b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f3b-139">Response</span></span>
<span data-ttu-id="01f3b-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01f3b-140">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f3b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="01f3b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="01f3b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f3b-142">Request</span></span>
<span data-ttu-id="01f3b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f3b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="01f3b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f3b-144">Response</span></span>
<span data-ttu-id="01f3b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01f3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



