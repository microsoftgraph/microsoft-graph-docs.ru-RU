---
title: действие updateStatus
description: Задайте состояние задачи и вложите заметку.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3bd6ccca0e6737c59773efd94bbacabc4d7bf01
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189782"
---
# <a name="updatestatus-action"></a><span data-ttu-id="aef9d-103">действие updateStatus</span><span class="sxs-lookup"><span data-stu-id="aef9d-103">updateStatus action</span></span>

> <span data-ttu-id="aef9d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aef9d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aef9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef9d-106">Задайте состояние задачи и вложите заметку.</span><span class="sxs-lookup"><span data-stu-id="aef9d-106">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aef9d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aef9d-107">Prerequisites</span></span>
<span data-ttu-id="aef9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aef9d-110">Permission type</span></span>|<span data-ttu-id="aef9d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aef9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aef9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aef9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aef9d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef9d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aef9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aef9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aef9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef9d-115">Not supported.</span></span>|
|<span data-ttu-id="aef9d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aef9d-116">Application</span></span>|<span data-ttu-id="aef9d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef9d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aef9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aef9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="aef9d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aef9d-119">Request headers</span></span>
|<span data-ttu-id="aef9d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aef9d-120">Header</span></span>|<span data-ttu-id="aef9d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aef9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aef9d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aef9d-122">Authorization</span></span>|<span data-ttu-id="aef9d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aef9d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aef9d-124">Accept</span></span>|<span data-ttu-id="aef9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aef9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef9d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aef9d-126">Request body</span></span>
<span data-ttu-id="aef9d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aef9d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aef9d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aef9d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aef9d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aef9d-129">Property</span></span>|<span data-ttu-id="aef9d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aef9d-130">Type</span></span>|<span data-ttu-id="aef9d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aef9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef9d-132">status</span><span class="sxs-lookup"><span data-stu-id="aef9d-132">status</span></span>|[<span data-ttu-id="aef9d-133">девицеаппманажементтаскстатус</span><span class="sxs-lookup"><span data-stu-id="aef9d-133">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="aef9d-134">Состояние</span><span class="sxs-lookup"><span data-stu-id="aef9d-134">The status</span></span>|
|<span data-ttu-id="aef9d-135">ноте</span><span class="sxs-lookup"><span data-stu-id="aef9d-135">note</span></span>|<span data-ttu-id="aef9d-136">String.</span><span class="sxs-lookup"><span data-stu-id="aef9d-136">String</span></span>|<span data-ttu-id="aef9d-137">Заметка</span><span class="sxs-lookup"><span data-stu-id="aef9d-137">The note</span></span>|



## <a name="response"></a><span data-ttu-id="aef9d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="aef9d-138">Response</span></span>
<span data-ttu-id="aef9d-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aef9d-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aef9d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="aef9d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="aef9d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef9d-141">Request</span></span>
<span data-ttu-id="aef9d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aef9d-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="aef9d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef9d-143">Response</span></span>
<span data-ttu-id="aef9d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aef9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




