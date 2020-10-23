---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78c6f5c581dbe78ab46c6356265e6c44d446ce11
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725949"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="c197a-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="c197a-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="c197a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c197a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c197a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c197a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c197a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c197a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c197a-107">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="c197a-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c197a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c197a-108">Prerequisites</span></span>
<span data-ttu-id="c197a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c197a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c197a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c197a-111">Permission type</span></span>|<span data-ttu-id="c197a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c197a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c197a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c197a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c197a-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c197a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c197a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197a-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c197a-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c197a-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c197a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c197a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c197a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c197a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c197a-119">Not supported.</span></span>|
|<span data-ttu-id="c197a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c197a-120">Application</span></span>||
| <span data-ttu-id="c197a-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c197a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c197a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197a-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c197a-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c197a-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c197a-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197a-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c197a-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c197a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c197a-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c197a-126">Request headers</span></span>
|<span data-ttu-id="c197a-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c197a-127">Header</span></span>|<span data-ttu-id="c197a-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c197a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c197a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c197a-129">Authorization</span></span>|<span data-ttu-id="c197a-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c197a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c197a-131">Accept</span><span class="sxs-lookup"><span data-stu-id="c197a-131">Accept</span></span>|<span data-ttu-id="c197a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c197a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c197a-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c197a-133">Request body</span></span>
<span data-ttu-id="c197a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c197a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c197a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c197a-135">Response</span></span>
<span data-ttu-id="c197a-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c197a-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c197a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c197a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c197a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c197a-138">Request</span></span>
<span data-ttu-id="c197a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c197a-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="c197a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c197a-140">Response</span></span>
<span data-ttu-id="c197a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c197a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








