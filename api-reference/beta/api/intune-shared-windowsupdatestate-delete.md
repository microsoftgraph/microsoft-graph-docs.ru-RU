---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55591b29710f956921445b4b06a1bc1929ea96e2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939334"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="25310-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="25310-103">Delete windowsUpdateState</span></span>

> <span data-ttu-id="25310-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25310-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25310-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25310-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25310-106">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="25310-106">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25310-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25310-107">Prerequisites</span></span>
<span data-ttu-id="25310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25310-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25310-110">Permission type</span></span>|<span data-ttu-id="25310-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25310-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25310-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25310-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="25310-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="25310-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="25310-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25310-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="25310-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="25310-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="25310-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25310-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25310-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25310-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25310-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25310-118">Not supported.</span></span>|
|<span data-ttu-id="25310-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25310-119">Application</span></span>||
| <span data-ttu-id="25310-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="25310-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="25310-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25310-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="25310-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="25310-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="25310-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25310-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25310-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25310-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="25310-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25310-125">Request headers</span></span>
|<span data-ttu-id="25310-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25310-126">Header</span></span>|<span data-ttu-id="25310-127">Значение</span><span class="sxs-lookup"><span data-stu-id="25310-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25310-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25310-128">Authorization</span></span>|<span data-ttu-id="25310-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25310-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25310-130">Accept</span><span class="sxs-lookup"><span data-stu-id="25310-130">Accept</span></span>|<span data-ttu-id="25310-131">application/json</span><span class="sxs-lookup"><span data-stu-id="25310-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25310-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25310-132">Request body</span></span>
<span data-ttu-id="25310-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25310-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25310-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="25310-134">Response</span></span>
<span data-ttu-id="25310-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25310-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25310-136">Пример</span><span class="sxs-lookup"><span data-stu-id="25310-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="25310-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="25310-137">Request</span></span>
<span data-ttu-id="25310-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25310-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="25310-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="25310-139">Response</span></span>
<span data-ttu-id="25310-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








