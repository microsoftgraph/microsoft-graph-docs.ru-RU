---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45a4e9caf2c32f65f2934636c51da6614ff66844
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537666"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="40c04-103">Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="40c04-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="40c04-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40c04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40c04-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40c04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40c04-106">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40c04-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40c04-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40c04-107">Prerequisites</span></span>
<span data-ttu-id="40c04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40c04-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40c04-110">Permission type</span></span>|<span data-ttu-id="40c04-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40c04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40c04-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40c04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40c04-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40c04-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40c04-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40c04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40c04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40c04-115">Not supported.</span></span>|
|<span data-ttu-id="40c04-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="40c04-116">Application</span></span>|<span data-ttu-id="40c04-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40c04-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40c04-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40c04-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="40c04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40c04-119">Request headers</span></span>
|<span data-ttu-id="40c04-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40c04-120">Header</span></span>|<span data-ttu-id="40c04-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40c04-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40c04-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40c04-122">Authorization</span></span>|<span data-ttu-id="40c04-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40c04-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40c04-124">Accept</span><span class="sxs-lookup"><span data-stu-id="40c04-124">Accept</span></span>|<span data-ttu-id="40c04-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40c04-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40c04-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40c04-126">Request body</span></span>
<span data-ttu-id="40c04-127">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40c04-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="40c04-128">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="40c04-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="40c04-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="40c04-129">Property</span></span>|<span data-ttu-id="40c04-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40c04-130">Type</span></span>|<span data-ttu-id="40c04-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40c04-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40c04-132">id</span><span class="sxs-lookup"><span data-stu-id="40c04-132">id</span></span>|<span data-ttu-id="40c04-133">String</span><span class="sxs-lookup"><span data-stu-id="40c04-133">String</span></span>|<span data-ttu-id="40c04-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40c04-134">Key of the entity.</span></span>|
|<span data-ttu-id="40c04-135">target</span><span class="sxs-lookup"><span data-stu-id="40c04-135">target</span></span>|[<span data-ttu-id="40c04-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="40c04-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="40c04-137">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="40c04-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="40c04-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="40c04-138">Response</span></span>
<span data-ttu-id="40c04-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40c04-139">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40c04-140">Пример</span><span class="sxs-lookup"><span data-stu-id="40c04-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="40c04-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="40c04-141">Request</span></span>
<span data-ttu-id="40c04-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40c04-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40c04-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="40c04-143">Response</span></span>
<span data-ttu-id="40c04-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40c04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






