---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bdaece991a477a3323919f4baf275b409b2cc0bc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863340"
---
# <a name="assign-action"></a><span data-ttu-id="5bbab-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="5bbab-103">assign action</span></span>

<span data-ttu-id="5bbab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bbab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bbab-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bbab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bbab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bbab-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5bbab-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bbab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5bbab-108">Prerequisites</span></span>
<span data-ttu-id="5bbab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bbab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbab-111">Permission type</span></span>|<span data-ttu-id="5bbab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bbab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bbab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bbab-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5bbab-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5bbab-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5bbab-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bbab-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5bbab-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bbab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bbab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbab-117">Not supported.</span></span>|
|<span data-ttu-id="5bbab-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="5bbab-118">Application</span></span>||
| <span data-ttu-id="5bbab-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5bbab-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5bbab-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bbab-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bbab-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bbab-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5bbab-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5bbab-122">Request headers</span></span>
|<span data-ttu-id="5bbab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bbab-123">Header</span></span>|<span data-ttu-id="5bbab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5bbab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bbab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bbab-125">Authorization</span></span>|<span data-ttu-id="5bbab-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bbab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bbab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5bbab-127">Accept</span></span>|<span data-ttu-id="5bbab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5bbab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bbab-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bbab-129">Request body</span></span>
<span data-ttu-id="5bbab-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bbab-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5bbab-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5bbab-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5bbab-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bbab-132">Property</span></span>|<span data-ttu-id="5bbab-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5bbab-133">Type</span></span>|<span data-ttu-id="5bbab-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5bbab-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bbab-135">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="5bbab-135">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="5bbab-136">[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bbab-136">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="5bbab-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5bbab-137">Not yet documented</span></span>|
|<span data-ttu-id="5bbab-138">assignments</span><span class="sxs-lookup"><span data-stu-id="5bbab-138">assignments</span></span>|<span data-ttu-id="5bbab-139">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bbab-139">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5bbab-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bbab-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5bbab-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbab-141">Response</span></span>
<span data-ttu-id="5bbab-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbab-142">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bbab-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5bbab-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bbab-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbab-144">Request</span></span>
<span data-ttu-id="5bbab-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bbab-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bbab-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbab-146">Response</span></span>
<span data-ttu-id="5bbab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bbab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







