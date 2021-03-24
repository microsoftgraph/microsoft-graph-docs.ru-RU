---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e77be56361eb85568fb0c959c696bd6c2351b068
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146449"
---
# <a name="assign-action"></a><span data-ttu-id="29b48-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="29b48-103">assign action</span></span>

<span data-ttu-id="29b48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29b48-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29b48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29b48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29b48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b48-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="29b48-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b48-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="29b48-108">Prerequisites</span></span>
<span data-ttu-id="29b48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29b48-111">Permission type</span></span>|<span data-ttu-id="29b48-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29b48-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b48-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29b48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29b48-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b48-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29b48-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29b48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29b48-116">Not supported.</span></span>|
|<span data-ttu-id="29b48-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="29b48-117">Application</span></span>|<span data-ttu-id="29b48-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b48-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29b48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="29b48-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="29b48-120">Request headers</span></span>
|<span data-ttu-id="29b48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29b48-121">Header</span></span>|<span data-ttu-id="29b48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="29b48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29b48-123">Authorization</span></span>|<span data-ttu-id="29b48-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29b48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29b48-125">Accept</span></span>|<span data-ttu-id="29b48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29b48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29b48-127">Request body</span></span>
<span data-ttu-id="29b48-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29b48-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="29b48-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="29b48-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="29b48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="29b48-130">Property</span></span>|<span data-ttu-id="29b48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="29b48-131">Type</span></span>|<span data-ttu-id="29b48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="29b48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b48-133">DeviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="29b48-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="29b48-134">[коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="29b48-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="29b48-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="29b48-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29b48-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="29b48-136">Response</span></span>
<span data-ttu-id="29b48-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29b48-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29b48-138">Пример</span><span class="sxs-lookup"><span data-stu-id="29b48-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b48-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="29b48-139">Request</span></span>
<span data-ttu-id="29b48-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29b48-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign

Content-type: application/json
Content-length: 756

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="29b48-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="29b48-141">Response</span></span>
<span data-ttu-id="29b48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29b48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




