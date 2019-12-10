---
title: Создание Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32b40173811a1869f6dfbecf3deeceb3e152feb3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938791"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="1e46d-103">Создание Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="1e46d-103">Create windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="1e46d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e46d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e46d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e46d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e46d-106">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1e46d-106">Create a new [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e46d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e46d-107">Prerequisites</span></span>
<span data-ttu-id="1e46d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e46d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e46d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e46d-110">Permission type</span></span>|<span data-ttu-id="1e46d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e46d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e46d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e46d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e46d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e46d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e46d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e46d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e46d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e46d-115">Not supported.</span></span>|
|<span data-ttu-id="1e46d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e46d-116">Application</span></span>|<span data-ttu-id="1e46d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e46d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e46d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e46d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1e46d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e46d-119">Request headers</span></span>
|<span data-ttu-id="1e46d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e46d-120">Header</span></span>|<span data-ttu-id="1e46d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1e46d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e46d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e46d-122">Authorization</span></span>|<span data-ttu-id="1e46d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e46d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e46d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1e46d-124">Accept</span></span>|<span data-ttu-id="1e46d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e46d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e46d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1e46d-126">Request body</span></span>
<span data-ttu-id="1e46d-127">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e46d-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyAssignment object.</span></span>

<span data-ttu-id="1e46d-128">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполициассигнмент.</span><span class="sxs-lookup"><span data-stu-id="1e46d-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyAssignment.</span></span>

|<span data-ttu-id="1e46d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e46d-129">Property</span></span>|<span data-ttu-id="1e46d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1e46d-130">Type</span></span>|<span data-ttu-id="1e46d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1e46d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e46d-132">id</span><span class="sxs-lookup"><span data-stu-id="1e46d-132">id</span></span>|<span data-ttu-id="1e46d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1e46d-133">String</span></span>|<span data-ttu-id="1e46d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e46d-134">Key of the entity.</span></span>|
|<span data-ttu-id="1e46d-135">target</span><span class="sxs-lookup"><span data-stu-id="1e46d-135">target</span></span>|[<span data-ttu-id="1e46d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1e46d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1e46d-137">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="1e46d-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="1e46d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e46d-138">Response</span></span>
<span data-ttu-id="1e46d-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e46d-139">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e46d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1e46d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e46d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e46d-141">Request</span></span>
<span data-ttu-id="1e46d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e46d-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e46d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e46d-143">Response</span></span>
<span data-ttu-id="1e46d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e46d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





