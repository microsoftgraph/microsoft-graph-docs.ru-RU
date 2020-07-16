---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00431a77432738eca351ccbe04d1a06c289db806
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791996"
---
# <a name="assign-action"></a><span data-ttu-id="36a04-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="36a04-103">assign action</span></span>

<span data-ttu-id="36a04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36a04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36a04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36a04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a04-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36a04-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36a04-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36a04-108">Prerequisites</span></span>
<span data-ttu-id="36a04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36a04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36a04-111">Permission type</span></span>|<span data-ttu-id="36a04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36a04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36a04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36a04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36a04-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36a04-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36a04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36a04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36a04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a04-116">Not supported.</span></span>|
|<span data-ttu-id="36a04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36a04-117">Application</span></span>|<span data-ttu-id="36a04-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36a04-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36a04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36a04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="36a04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36a04-120">Request headers</span></span>
|<span data-ttu-id="36a04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36a04-121">Header</span></span>|<span data-ttu-id="36a04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36a04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36a04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36a04-123">Authorization</span></span>|<span data-ttu-id="36a04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36a04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36a04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36a04-125">Accept</span></span>|<span data-ttu-id="36a04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36a04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36a04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36a04-127">Request body</span></span>
<span data-ttu-id="36a04-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36a04-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="36a04-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="36a04-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="36a04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36a04-130">Property</span></span>|<span data-ttu-id="36a04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36a04-131">Type</span></span>|<span data-ttu-id="36a04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36a04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a04-133">assignments</span><span class="sxs-lookup"><span data-stu-id="36a04-133">assignments</span></span>|<span data-ttu-id="36a04-134">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="36a04-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="36a04-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36a04-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="36a04-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="36a04-136">Response</span></span>
<span data-ttu-id="36a04-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36a04-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a04-138">Пример</span><span class="sxs-lookup"><span data-stu-id="36a04-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="36a04-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="36a04-139">Request</span></span>
<span data-ttu-id="36a04-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36a04-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 513

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="36a04-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a04-141">Response</span></span>
<span data-ttu-id="36a04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36a04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



