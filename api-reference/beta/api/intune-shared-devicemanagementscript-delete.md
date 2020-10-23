---
title: Удаление deviceManagementScript
description: Удаляет объект deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3cc312079c75ac87ea117efdeb56cf3d16fc727
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725956"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="d2759-103">Удаление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="d2759-103">Delete deviceManagementScript</span></span>

<span data-ttu-id="d2759-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2759-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2759-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2759-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2759-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2759-107">Удаляет объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="d2759-107">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2759-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2759-108">Prerequisites</span></span>
<span data-ttu-id="d2759-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2759-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2759-111">Permission type</span></span>|<span data-ttu-id="d2759-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2759-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2759-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d2759-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d2759-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d2759-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2759-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d2759-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d2759-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d2759-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2759-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2759-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2759-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2759-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2759-119">Not supported.</span></span>|
|<span data-ttu-id="d2759-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2759-120">Application</span></span>||
| <span data-ttu-id="d2759-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d2759-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d2759-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2759-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d2759-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d2759-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d2759-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2759-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2759-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2759-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="d2759-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2759-126">Request headers</span></span>
|<span data-ttu-id="d2759-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2759-127">Header</span></span>|<span data-ttu-id="d2759-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d2759-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2759-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2759-129">Authorization</span></span>|<span data-ttu-id="d2759-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2759-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2759-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d2759-131">Accept</span></span>|<span data-ttu-id="d2759-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d2759-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2759-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2759-133">Request body</span></span>
<span data-ttu-id="d2759-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2759-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2759-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2759-135">Response</span></span>
<span data-ttu-id="d2759-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2759-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2759-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d2759-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2759-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2759-138">Request</span></span>
<span data-ttu-id="d2759-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2759-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="d2759-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2759-140">Response</span></span>
<span data-ttu-id="d2759-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2759-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








