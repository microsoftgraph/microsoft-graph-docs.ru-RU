---
title: действие updateStatus
description: Установите состояние задачи и приложите примечание.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a03d26b3002e39ae27c0920bc95c5ce5f569584d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134849"
---
# <a name="updatestatus-action"></a><span data-ttu-id="75938-103">действие updateStatus</span><span class="sxs-lookup"><span data-stu-id="75938-103">updateStatus action</span></span>

<span data-ttu-id="75938-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75938-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75938-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75938-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75938-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75938-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75938-107">Установите состояние задачи и приложите примечание.</span><span class="sxs-lookup"><span data-stu-id="75938-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75938-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75938-108">Prerequisites</span></span>
<span data-ttu-id="75938-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75938-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75938-111">Permission type</span></span>|<span data-ttu-id="75938-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75938-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75938-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75938-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75938-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75938-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75938-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75938-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75938-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75938-116">Not supported.</span></span>|
|<span data-ttu-id="75938-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75938-117">Application</span></span>|<span data-ttu-id="75938-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75938-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75938-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75938-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="75938-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75938-120">Request headers</span></span>
|<span data-ttu-id="75938-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75938-121">Header</span></span>|<span data-ttu-id="75938-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75938-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75938-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75938-123">Authorization</span></span>|<span data-ttu-id="75938-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75938-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75938-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75938-125">Accept</span></span>|<span data-ttu-id="75938-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75938-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75938-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75938-127">Request body</span></span>
<span data-ttu-id="75938-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75938-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75938-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="75938-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75938-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75938-130">Property</span></span>|<span data-ttu-id="75938-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75938-131">Type</span></span>|<span data-ttu-id="75938-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75938-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75938-133">status</span><span class="sxs-lookup"><span data-stu-id="75938-133">status</span></span>|[<span data-ttu-id="75938-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="75938-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="75938-135">Состояние</span><span class="sxs-lookup"><span data-stu-id="75938-135">The status</span></span>|
|<span data-ttu-id="75938-136">примечание</span><span class="sxs-lookup"><span data-stu-id="75938-136">note</span></span>|<span data-ttu-id="75938-137">Строка</span><span class="sxs-lookup"><span data-stu-id="75938-137">String</span></span>|<span data-ttu-id="75938-138">Примечание</span><span class="sxs-lookup"><span data-stu-id="75938-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="75938-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="75938-139">Response</span></span>
<span data-ttu-id="75938-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75938-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75938-141">Пример</span><span class="sxs-lookup"><span data-stu-id="75938-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="75938-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="75938-142">Request</span></span>
<span data-ttu-id="75938-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75938-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="75938-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="75938-144">Response</span></span>
<span data-ttu-id="75938-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75938-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




