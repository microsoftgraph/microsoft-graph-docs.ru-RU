---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7fde6cc402f783f6402744123a4fef6fca6f691
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380951"
---
# <a name="assign-action"></a><span data-ttu-id="9b825-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="9b825-103">assign action</span></span>

<span data-ttu-id="9b825-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b825-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b825-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b825-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b825-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9b825-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b825-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9b825-108">Prerequisites</span></span>
<span data-ttu-id="9b825-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b825-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b825-111">Permission type</span></span>|<span data-ttu-id="9b825-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b825-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b825-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b825-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b825-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b825-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b825-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b825-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b825-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b825-116">Not supported.</span></span>|
|<span data-ttu-id="9b825-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b825-117">Application</span></span>|<span data-ttu-id="9b825-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b825-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b825-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b825-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9b825-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b825-120">Request headers</span></span>
|<span data-ttu-id="9b825-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b825-121">Header</span></span>|<span data-ttu-id="9b825-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b825-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b825-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b825-123">Authorization</span></span>|<span data-ttu-id="9b825-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b825-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b825-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b825-125">Accept</span></span>|<span data-ttu-id="9b825-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b825-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b825-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b825-127">Request body</span></span>
<span data-ttu-id="9b825-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b825-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9b825-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9b825-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9b825-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b825-130">Property</span></span>|<span data-ttu-id="9b825-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b825-131">Type</span></span>|<span data-ttu-id="9b825-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b825-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b825-133">девицехеалсскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="9b825-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="9b825-134">Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b825-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="9b825-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9b825-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b825-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b825-136">Response</span></span>
<span data-ttu-id="9b825-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b825-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9b825-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9b825-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b825-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b825-139">Request</span></span>
<span data-ttu-id="9b825-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b825-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 419

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9b825-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b825-141">Response</span></span>
<span data-ttu-id="9b825-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



