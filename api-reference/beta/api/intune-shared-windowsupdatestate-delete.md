---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6a7c9d4b2b08db57d3c25f6d4d3e7d9d46435a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967026"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="38e58-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="38e58-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="38e58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38e58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38e58-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38e58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38e58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38e58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38e58-107">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="38e58-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38e58-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38e58-108">Prerequisites</span></span>
<span data-ttu-id="38e58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38e58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38e58-111">Permission type</span></span>|<span data-ttu-id="38e58-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38e58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38e58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38e58-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="38e58-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="38e58-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="38e58-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e58-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="38e58-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="38e58-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="38e58-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e58-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38e58-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38e58-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38e58-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38e58-119">Not supported.</span></span>|
|<span data-ttu-id="38e58-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38e58-120">Application</span></span>||
| <span data-ttu-id="38e58-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="38e58-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="38e58-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e58-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="38e58-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="38e58-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="38e58-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e58-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38e58-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38e58-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="38e58-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38e58-126">Request headers</span></span>
|<span data-ttu-id="38e58-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38e58-127">Header</span></span>|<span data-ttu-id="38e58-128">Значение</span><span class="sxs-lookup"><span data-stu-id="38e58-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38e58-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="38e58-129">Authorization</span></span>|<span data-ttu-id="38e58-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38e58-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38e58-131">Accept</span><span class="sxs-lookup"><span data-stu-id="38e58-131">Accept</span></span>|<span data-ttu-id="38e58-132">application/json</span><span class="sxs-lookup"><span data-stu-id="38e58-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38e58-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38e58-133">Request body</span></span>
<span data-ttu-id="38e58-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38e58-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38e58-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="38e58-135">Response</span></span>
<span data-ttu-id="38e58-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="38e58-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38e58-137">Пример</span><span class="sxs-lookup"><span data-stu-id="38e58-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="38e58-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="38e58-138">Request</span></span>
<span data-ttu-id="38e58-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38e58-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="38e58-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="38e58-140">Response</span></span>
<span data-ttu-id="38e58-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38e58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









