---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 725e751d17493ccadb7509fba8d21b9e8e7e2672
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295770"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="84b8d-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="84b8d-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="84b8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84b8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84b8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84b8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84b8d-107">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="84b8d-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84b8d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84b8d-108">Prerequisites</span></span>
<span data-ttu-id="84b8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84b8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b8d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84b8d-111">Permission type</span></span>|<span data-ttu-id="84b8d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84b8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84b8d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84b8d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="84b8d-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="84b8d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="84b8d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b8d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="84b8d-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="84b8d-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="84b8d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b8d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84b8d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84b8d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84b8d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b8d-119">Not supported.</span></span>|
|<span data-ttu-id="84b8d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84b8d-120">Application</span></span>||
| <span data-ttu-id="84b8d-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="84b8d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="84b8d-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b8d-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="84b8d-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="84b8d-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="84b8d-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b8d-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84b8d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84b8d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="84b8d-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84b8d-126">Request headers</span></span>
|<span data-ttu-id="84b8d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84b8d-127">Header</span></span>|<span data-ttu-id="84b8d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="84b8d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84b8d-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84b8d-129">Authorization</span></span>|<span data-ttu-id="84b8d-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84b8d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84b8d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="84b8d-131">Accept</span></span>|<span data-ttu-id="84b8d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="84b8d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84b8d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84b8d-133">Request body</span></span>
<span data-ttu-id="84b8d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84b8d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84b8d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84b8d-135">Response</span></span>
<span data-ttu-id="84b8d-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="84b8d-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84b8d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="84b8d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="84b8d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="84b8d-138">Request</span></span>
<span data-ttu-id="84b8d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84b8d-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="84b8d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="84b8d-140">Response</span></span>
<span data-ttu-id="84b8d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84b8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







