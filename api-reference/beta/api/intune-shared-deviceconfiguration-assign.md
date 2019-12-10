---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5ff7624dac19c58a52a176c0407efa03984d2a0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940091"
---
# <a name="assign-action"></a><span data-ttu-id="effab-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="effab-103">assign action</span></span>

> <span data-ttu-id="effab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="effab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="effab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="effab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="effab-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="effab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="effab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="effab-107">Prerequisites</span></span>
<span data-ttu-id="effab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="effab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="effab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="effab-110">Permission type</span></span>|<span data-ttu-id="effab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="effab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="effab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="effab-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="effab-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="effab-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="effab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="effab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="effab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="effab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="effab-116">Not supported.</span></span>|
|<span data-ttu-id="effab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="effab-117">Application</span></span>||
| <span data-ttu-id="effab-118">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="effab-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="effab-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="effab-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="effab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="effab-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="effab-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="effab-121">Request headers</span></span>
|<span data-ttu-id="effab-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="effab-122">Header</span></span>|<span data-ttu-id="effab-123">Значение</span><span class="sxs-lookup"><span data-stu-id="effab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="effab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="effab-124">Authorization</span></span>|<span data-ttu-id="effab-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="effab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="effab-126">Accept</span><span class="sxs-lookup"><span data-stu-id="effab-126">Accept</span></span>|<span data-ttu-id="effab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="effab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="effab-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="effab-128">Request body</span></span>
<span data-ttu-id="effab-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="effab-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="effab-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="effab-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="effab-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="effab-131">Property</span></span>|<span data-ttu-id="effab-132">Тип</span><span class="sxs-lookup"><span data-stu-id="effab-132">Type</span></span>|<span data-ttu-id="effab-133">Описание</span><span class="sxs-lookup"><span data-stu-id="effab-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="effab-134">девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="effab-134">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="effab-135">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="effab-135">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="effab-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="effab-136">Not yet documented</span></span>|
|<span data-ttu-id="effab-137">assignments</span><span class="sxs-lookup"><span data-stu-id="effab-137">assignments</span></span>|<span data-ttu-id="effab-138">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="effab-138">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="effab-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="effab-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="effab-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="effab-140">Response</span></span>
<span data-ttu-id="effab-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="effab-141">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="effab-142">Пример</span><span class="sxs-lookup"><span data-stu-id="effab-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="effab-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="effab-143">Request</span></span>
<span data-ttu-id="effab-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="effab-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="effab-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="effab-145">Response</span></span>
<span data-ttu-id="effab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="effab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








