---
title: Удаление deviceManagementIntentDeviceState
description: Удаляет устройствоManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3292e69cbed24bfb8faaddfedcbe22ad84ce69d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132025"
---
# <a name="delete-devicemanagementintentdevicestate"></a><span data-ttu-id="52dfe-103">Удаление deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="52dfe-103">Delete deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="52dfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52dfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52dfe-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52dfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52dfe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52dfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52dfe-107">Удаляет [устройствоManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="52dfe-107">Deletes a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52dfe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52dfe-108">Prerequisites</span></span>
<span data-ttu-id="52dfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52dfe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52dfe-111">Permission type</span></span>|<span data-ttu-id="52dfe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52dfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52dfe-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52dfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52dfe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52dfe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52dfe-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52dfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52dfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52dfe-116">Not supported.</span></span>|
|<span data-ttu-id="52dfe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="52dfe-117">Application</span></span>|<span data-ttu-id="52dfe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52dfe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52dfe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52dfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="52dfe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52dfe-120">Request headers</span></span>
|<span data-ttu-id="52dfe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52dfe-121">Header</span></span>|<span data-ttu-id="52dfe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52dfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52dfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52dfe-123">Authorization</span></span>|<span data-ttu-id="52dfe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52dfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52dfe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52dfe-125">Accept</span></span>|<span data-ttu-id="52dfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52dfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52dfe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52dfe-127">Request body</span></span>
<span data-ttu-id="52dfe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52dfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52dfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="52dfe-129">Response</span></span>
<span data-ttu-id="52dfe-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52dfe-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52dfe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="52dfe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="52dfe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="52dfe-132">Request</span></span>
<span data-ttu-id="52dfe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52dfe-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="52dfe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="52dfe-134">Response</span></span>
<span data-ttu-id="52dfe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52dfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




