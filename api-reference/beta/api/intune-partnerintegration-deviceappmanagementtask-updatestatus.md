---
title: действие updateStatus
description: Задайте состояние задачи и вложите заметку.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6e8bc97b8c5ef9d54b7d1a753b1bd4602b2eeb4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726047"
---
# <a name="updatestatus-action"></a><span data-ttu-id="32964-103">действие updateStatus</span><span class="sxs-lookup"><span data-stu-id="32964-103">updateStatus action</span></span>

<span data-ttu-id="32964-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32964-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32964-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32964-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32964-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32964-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32964-107">Задайте состояние задачи и вложите заметку.</span><span class="sxs-lookup"><span data-stu-id="32964-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32964-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32964-108">Prerequisites</span></span>
<span data-ttu-id="32964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32964-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32964-111">Permission type</span></span>|<span data-ttu-id="32964-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32964-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32964-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32964-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32964-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32964-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32964-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32964-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32964-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32964-116">Not supported.</span></span>|
|<span data-ttu-id="32964-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32964-117">Application</span></span>|<span data-ttu-id="32964-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32964-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32964-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32964-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="32964-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32964-120">Request headers</span></span>
|<span data-ttu-id="32964-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32964-121">Header</span></span>|<span data-ttu-id="32964-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32964-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32964-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32964-123">Authorization</span></span>|<span data-ttu-id="32964-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32964-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32964-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32964-125">Accept</span></span>|<span data-ttu-id="32964-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32964-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32964-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32964-127">Request body</span></span>
<span data-ttu-id="32964-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32964-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32964-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="32964-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32964-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32964-130">Property</span></span>|<span data-ttu-id="32964-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32964-131">Type</span></span>|<span data-ttu-id="32964-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32964-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32964-133">status</span><span class="sxs-lookup"><span data-stu-id="32964-133">status</span></span>|[<span data-ttu-id="32964-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="32964-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="32964-135">Состояние</span><span class="sxs-lookup"><span data-stu-id="32964-135">The status</span></span>|
|<span data-ttu-id="32964-136">ноте</span><span class="sxs-lookup"><span data-stu-id="32964-136">note</span></span>|<span data-ttu-id="32964-137">Строка</span><span class="sxs-lookup"><span data-stu-id="32964-137">String</span></span>|<span data-ttu-id="32964-138">Заметка</span><span class="sxs-lookup"><span data-stu-id="32964-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="32964-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="32964-139">Response</span></span>
<span data-ttu-id="32964-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32964-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32964-141">Пример</span><span class="sxs-lookup"><span data-stu-id="32964-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="32964-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="32964-142">Request</span></span>
<span data-ttu-id="32964-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32964-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="32964-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="32964-144">Response</span></span>
<span data-ttu-id="32964-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





