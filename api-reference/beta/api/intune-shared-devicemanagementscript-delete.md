---
title: Удаление deviceManagementScript
description: Удаляет объект deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebdd34050fb625160ea97ef0cd54a3c543172e2d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538156"
---
# <a name="delete-devicemanagementscript"></a><span data-ttu-id="5c5cd-103">Удаление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="5c5cd-103">Delete deviceManagementScript</span></span>

> <span data-ttu-id="5c5cd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c5cd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c5cd-106">Удаляет объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="5c5cd-106">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c5cd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c5cd-107">Prerequisites</span></span>
<span data-ttu-id="5c5cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5cd-110">Permission type</span></span>|<span data-ttu-id="5c5cd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c5cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c5cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c5cd-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5c5cd-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5c5cd-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5c5cd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5cd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5c5cd-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5c5cd-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5c5cd-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5cd-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c5cd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c5cd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c5cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-118">Not supported.</span></span>|
|<span data-ttu-id="5c5cd-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="5c5cd-119">Application</span></span>||
| <span data-ttu-id="5c5cd-120">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5c5cd-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5c5cd-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5cd-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5c5cd-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5c5cd-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5c5cd-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5cd-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c5cd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c5cd-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="5c5cd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c5cd-125">Request headers</span></span>
|<span data-ttu-id="5c5cd-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c5cd-126">Header</span></span>|<span data-ttu-id="5c5cd-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5c5cd-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c5cd-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c5cd-128">Authorization</span></span>|<span data-ttu-id="5c5cd-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c5cd-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5c5cd-130">Accept</span></span>|<span data-ttu-id="5c5cd-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5c5cd-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5cd-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c5cd-132">Request body</span></span>
<span data-ttu-id="5c5cd-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5cd-134">Response</span></span>
<span data-ttu-id="5c5cd-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c5cd-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5c5cd-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c5cd-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5cd-137">Request</span></span>
<span data-ttu-id="5c5cd-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="5c5cd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5cd-139">Response</span></span>
<span data-ttu-id="5c5cd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c5cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






