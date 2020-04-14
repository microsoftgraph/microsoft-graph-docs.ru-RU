---
title: действие updateStatus
description: Задайте состояние задачи и вложите заметку.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f48563ae657934a84441648a314b93ac4af2656
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445308"
---
# <a name="updatestatus-action"></a><span data-ttu-id="2777d-103">действие updateStatus</span><span class="sxs-lookup"><span data-stu-id="2777d-103">updateStatus action</span></span>

<span data-ttu-id="2777d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2777d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2777d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2777d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2777d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2777d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2777d-107">Задайте состояние задачи и вложите заметку.</span><span class="sxs-lookup"><span data-stu-id="2777d-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2777d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2777d-108">Prerequisites</span></span>
<span data-ttu-id="2777d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2777d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2777d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2777d-111">Permission type</span></span>|<span data-ttu-id="2777d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2777d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2777d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2777d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2777d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2777d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2777d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2777d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2777d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2777d-116">Not supported.</span></span>|
|<span data-ttu-id="2777d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2777d-117">Application</span></span>|<span data-ttu-id="2777d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2777d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2777d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2777d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="2777d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2777d-120">Request headers</span></span>
|<span data-ttu-id="2777d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2777d-121">Header</span></span>|<span data-ttu-id="2777d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2777d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2777d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2777d-123">Authorization</span></span>|<span data-ttu-id="2777d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2777d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2777d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2777d-125">Accept</span></span>|<span data-ttu-id="2777d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2777d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2777d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2777d-127">Request body</span></span>
<span data-ttu-id="2777d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2777d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2777d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2777d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2777d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2777d-130">Property</span></span>|<span data-ttu-id="2777d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2777d-131">Type</span></span>|<span data-ttu-id="2777d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2777d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2777d-133">status</span><span class="sxs-lookup"><span data-stu-id="2777d-133">status</span></span>|[<span data-ttu-id="2777d-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="2777d-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="2777d-135">Состояние</span><span class="sxs-lookup"><span data-stu-id="2777d-135">The status</span></span>|
|<span data-ttu-id="2777d-136">ноте</span><span class="sxs-lookup"><span data-stu-id="2777d-136">note</span></span>|<span data-ttu-id="2777d-137">String</span><span class="sxs-lookup"><span data-stu-id="2777d-137">String</span></span>|<span data-ttu-id="2777d-138">Заметка</span><span class="sxs-lookup"><span data-stu-id="2777d-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="2777d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2777d-139">Response</span></span>
<span data-ttu-id="2777d-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2777d-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2777d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2777d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2777d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2777d-142">Request</span></span>
<span data-ttu-id="2777d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2777d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="2777d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2777d-144">Response</span></span>
<span data-ttu-id="2777d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2777d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



