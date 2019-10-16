---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf428298964bc97351fb74190de15a424b64e50d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531814"
---
# <a name="assign-action"></a><span data-ttu-id="8314c-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="8314c-103">assign action</span></span>

> <span data-ttu-id="8314c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8314c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8314c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8314c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8314c-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8314c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8314c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8314c-107">Prerequisites</span></span>
<span data-ttu-id="8314c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8314c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8314c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8314c-110">Permission type</span></span>|<span data-ttu-id="8314c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8314c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8314c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8314c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8314c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8314c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8314c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8314c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8314c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8314c-115">Not supported.</span></span>|
|<span data-ttu-id="8314c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8314c-116">Application</span></span>|<span data-ttu-id="8314c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8314c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8314c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8314c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="8314c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8314c-119">Request headers</span></span>
|<span data-ttu-id="8314c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8314c-120">Header</span></span>|<span data-ttu-id="8314c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8314c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8314c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8314c-122">Authorization</span></span>|<span data-ttu-id="8314c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8314c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8314c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8314c-124">Accept</span></span>|<span data-ttu-id="8314c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8314c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8314c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8314c-126">Request body</span></span>
<span data-ttu-id="8314c-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8314c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8314c-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8314c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8314c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8314c-129">Property</span></span>|<span data-ttu-id="8314c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8314c-130">Type</span></span>|<span data-ttu-id="8314c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8314c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8314c-132">девицехеалсскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="8314c-132">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="8314c-133">Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8314c-133">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="8314c-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8314c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8314c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8314c-135">Response</span></span>
<span data-ttu-id="8314c-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8314c-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8314c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="8314c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8314c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8314c-138">Request</span></span>
<span data-ttu-id="8314c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8314c-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8314c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8314c-140">Response</span></span>
<span data-ttu-id="8314c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8314c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






