---
title: Удаление Виндовсупдатестате
description: Удаляет объект Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dda36872332e6a957a7315df26a114dfbafd0062
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456216"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="39226-103">Удаление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="39226-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="39226-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39226-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39226-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39226-107">Удаляет объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="39226-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39226-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39226-108">Prerequisites</span></span>
<span data-ttu-id="39226-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39226-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39226-111">Permission type</span></span>|<span data-ttu-id="39226-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39226-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39226-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="39226-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="39226-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="39226-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39226-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="39226-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="39226-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="39226-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39226-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39226-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39226-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39226-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39226-119">Not supported.</span></span>|
|<span data-ttu-id="39226-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39226-120">Application</span></span>||
| <span data-ttu-id="39226-121">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="39226-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="39226-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39226-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="39226-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="39226-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="39226-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39226-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39226-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39226-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="39226-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39226-126">Request headers</span></span>
|<span data-ttu-id="39226-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39226-127">Header</span></span>|<span data-ttu-id="39226-128">Значение</span><span class="sxs-lookup"><span data-stu-id="39226-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39226-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39226-129">Authorization</span></span>|<span data-ttu-id="39226-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39226-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39226-131">Accept</span><span class="sxs-lookup"><span data-stu-id="39226-131">Accept</span></span>|<span data-ttu-id="39226-132">application/json</span><span class="sxs-lookup"><span data-stu-id="39226-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39226-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39226-133">Request body</span></span>
<span data-ttu-id="39226-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39226-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39226-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="39226-135">Response</span></span>
<span data-ttu-id="39226-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39226-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39226-137">Пример</span><span class="sxs-lookup"><span data-stu-id="39226-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="39226-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="39226-138">Request</span></span>
<span data-ttu-id="39226-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39226-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="39226-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="39226-140">Response</span></span>
<span data-ttu-id="39226-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39226-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






