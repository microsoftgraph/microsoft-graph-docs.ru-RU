---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 812a5cec0c85529759ed36606614cb7faeb8dc78
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800440"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="24e16-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="24e16-103">Delete windowsUpdateState</span></span>

> <span data-ttu-id="24e16-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24e16-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24e16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24e16-106">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="24e16-106">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24e16-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24e16-107">Prerequisites</span></span>
<span data-ttu-id="24e16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24e16-110">Permission type</span></span>|<span data-ttu-id="24e16-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24e16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24e16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24e16-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="24e16-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="24e16-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="24e16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24e16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="24e16-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="24e16-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="24e16-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24e16-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24e16-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24e16-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24e16-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24e16-118">Not supported.</span></span>|
|<span data-ttu-id="24e16-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="24e16-119">Application</span></span>||
| <span data-ttu-id="24e16-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="24e16-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="24e16-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24e16-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="24e16-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="24e16-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="24e16-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24e16-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24e16-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24e16-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="24e16-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24e16-125">Request headers</span></span>
|<span data-ttu-id="24e16-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24e16-126">Header</span></span>|<span data-ttu-id="24e16-127">Значение</span><span class="sxs-lookup"><span data-stu-id="24e16-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24e16-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="24e16-128">Authorization</span></span>|<span data-ttu-id="24e16-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24e16-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24e16-130">Accept</span><span class="sxs-lookup"><span data-stu-id="24e16-130">Accept</span></span>|<span data-ttu-id="24e16-131">application/json</span><span class="sxs-lookup"><span data-stu-id="24e16-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24e16-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24e16-132">Request body</span></span>
<span data-ttu-id="24e16-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24e16-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e16-134">Response</span></span>
<span data-ttu-id="24e16-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24e16-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24e16-136">Пример</span><span class="sxs-lookup"><span data-stu-id="24e16-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="24e16-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="24e16-137">Request</span></span>
<span data-ttu-id="24e16-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24e16-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="24e16-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="24e16-139">Response</span></span>
<span data-ttu-id="24e16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24e16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







