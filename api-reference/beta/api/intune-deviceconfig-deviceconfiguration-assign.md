---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11d0ab54c4f339ceb30fce5d07d4a2dc7457ec13
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927568"
---
# <a name="assign-action"></a><span data-ttu-id="e89fa-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e89fa-103">assign action</span></span>

> <span data-ttu-id="e89fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e89fa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e89fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e89fa-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e89fa-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e89fa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e89fa-107">Prerequisites</span></span>
<span data-ttu-id="e89fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e89fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e89fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e89fa-110">Permission type</span></span>|<span data-ttu-id="e89fa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e89fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e89fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e89fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e89fa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e89fa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e89fa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e89fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e89fa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89fa-115">Not supported.</span></span>|
|<span data-ttu-id="e89fa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e89fa-116">Application</span></span>|<span data-ttu-id="e89fa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e89fa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e89fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e89fa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e89fa-119">Request headers</span></span>
|<span data-ttu-id="e89fa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e89fa-120">Header</span></span>|<span data-ttu-id="e89fa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e89fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e89fa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e89fa-122">Authorization</span></span>|<span data-ttu-id="e89fa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e89fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e89fa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e89fa-124">Accept</span></span>|<span data-ttu-id="e89fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e89fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e89fa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e89fa-126">Request body</span></span>
<span data-ttu-id="e89fa-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e89fa-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e89fa-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e89fa-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e89fa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89fa-129">Property</span></span>|<span data-ttu-id="e89fa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e89fa-130">Type</span></span>|<span data-ttu-id="e89fa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e89fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e89fa-132">Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="e89fa-132">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="e89fa-133">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e89fa-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="e89fa-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e89fa-134">Not yet documented</span></span>|
|<span data-ttu-id="e89fa-135">assignments</span><span class="sxs-lookup"><span data-stu-id="e89fa-135">assignments</span></span>|<span data-ttu-id="e89fa-136">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e89fa-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e89fa-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e89fa-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e89fa-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89fa-138">Response</span></span>
<span data-ttu-id="e89fa-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e89fa-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89fa-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e89fa-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e89fa-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e89fa-141">Request</span></span>
<span data-ttu-id="e89fa-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e89fa-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e89fa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89fa-143">Response</span></span>
<span data-ttu-id="e89fa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e89fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




