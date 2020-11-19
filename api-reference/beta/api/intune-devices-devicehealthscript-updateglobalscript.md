---
title: действие Упдатеглобалскрипт
description: Обновление сценария работоспособности собственного устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02fee7b1ef4258dcc3eca337b88ef263a23210f5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228927"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="5a4a3-103">действие Упдатеглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="5a4a3-103">updateGlobalScript action</span></span>

<span data-ttu-id="5a4a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a4a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a4a3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a4a3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a4a3-107">Обновление сценария работоспособности собственного устройства</span><span class="sxs-lookup"><span data-stu-id="5a4a3-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a4a3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a4a3-108">Prerequisites</span></span>
<span data-ttu-id="5a4a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a4a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a4a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a4a3-111">Permission type</span></span>|<span data-ttu-id="5a4a3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a4a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a4a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a4a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a4a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a4a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a4a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a4a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a4a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-116">Not supported.</span></span>|
|<span data-ttu-id="5a4a3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5a4a3-117">Application</span></span>|<span data-ttu-id="5a4a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a4a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a4a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a4a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="5a4a3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a4a3-120">Request headers</span></span>
|<span data-ttu-id="5a4a3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a4a3-121">Header</span></span>|<span data-ttu-id="5a4a3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5a4a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a4a3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a4a3-123">Authorization</span></span>|<span data-ttu-id="5a4a3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a4a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5a4a3-125">Accept</span></span>|<span data-ttu-id="5a4a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a4a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a4a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a4a3-127">Request body</span></span>
<span data-ttu-id="5a4a3-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5a4a3-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5a4a3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a4a3-130">Property</span></span>|<span data-ttu-id="5a4a3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5a4a3-131">Type</span></span>|<span data-ttu-id="5a4a3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a4a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a4a3-133">version</span><span class="sxs-lookup"><span data-stu-id="5a4a3-133">version</span></span>|<span data-ttu-id="5a4a3-134">String</span><span class="sxs-lookup"><span data-stu-id="5a4a3-134">String</span></span>|<span data-ttu-id="5a4a3-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5a4a3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4a3-136">Response</span></span>
<span data-ttu-id="5a4a3-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a4a3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5a4a3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a4a3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a4a3-139">Request</span></span>
<span data-ttu-id="5a4a3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5a4a3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4a3-141">Response</span></span>
<span data-ttu-id="5a4a3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a4a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```




