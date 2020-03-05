---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1198468213fa9f3c590d13b8683409bdf0cf16d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458702"
---
# <a name="assign-action"></a><span data-ttu-id="642ad-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="642ad-103">assign action</span></span>

<span data-ttu-id="642ad-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="642ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="642ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="642ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="642ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="642ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="642ad-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="642ad-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="642ad-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="642ad-108">Prerequisites</span></span>
<span data-ttu-id="642ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="642ad-111">Permission type</span></span>|<span data-ttu-id="642ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="642ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="642ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="642ad-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="642ad-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="642ad-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="642ad-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642ad-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="642ad-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="642ad-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="642ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="642ad-117">Not supported.</span></span>|
|<span data-ttu-id="642ad-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="642ad-118">Application</span></span>||
| <span data-ttu-id="642ad-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="642ad-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="642ad-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642ad-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="642ad-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="642ad-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="642ad-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="642ad-122">Request headers</span></span>
|<span data-ttu-id="642ad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="642ad-123">Header</span></span>|<span data-ttu-id="642ad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="642ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="642ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="642ad-125">Authorization</span></span>|<span data-ttu-id="642ad-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="642ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="642ad-127">Accept</span><span class="sxs-lookup"><span data-stu-id="642ad-127">Accept</span></span>|<span data-ttu-id="642ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="642ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="642ad-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="642ad-129">Request body</span></span>
<span data-ttu-id="642ad-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="642ad-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="642ad-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="642ad-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="642ad-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="642ad-132">Property</span></span>|<span data-ttu-id="642ad-133">Тип</span><span class="sxs-lookup"><span data-stu-id="642ad-133">Type</span></span>|<span data-ttu-id="642ad-134">Описание</span><span class="sxs-lookup"><span data-stu-id="642ad-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="642ad-135">девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="642ad-135">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="642ad-136">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="642ad-136">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="642ad-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="642ad-137">Not yet documented</span></span>|
|<span data-ttu-id="642ad-138">assignments</span><span class="sxs-lookup"><span data-stu-id="642ad-138">assignments</span></span>|<span data-ttu-id="642ad-139">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="642ad-139">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="642ad-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="642ad-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="642ad-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="642ad-141">Response</span></span>
<span data-ttu-id="642ad-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="642ad-142">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642ad-143">Пример</span><span class="sxs-lookup"><span data-stu-id="642ad-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="642ad-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="642ad-144">Request</span></span>
<span data-ttu-id="642ad-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="642ad-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 617

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
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="642ad-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="642ad-146">Response</span></span>
<span data-ttu-id="642ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="642ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```








