---
title: действие Упдатеглобалскрипт
description: Обновление сценария работоспособности собственного устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42cd16873e374dfbc301674c2a7c76527311581a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426350"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="58e22-103">действие Упдатеглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="58e22-103">updateGlobalScript action</span></span>

<span data-ttu-id="58e22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58e22-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58e22-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58e22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58e22-107">Обновление сценария работоспособности собственного устройства</span><span class="sxs-lookup"><span data-stu-id="58e22-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58e22-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58e22-108">Prerequisites</span></span>
<span data-ttu-id="58e22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e22-111">Permission type</span></span>|<span data-ttu-id="58e22-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58e22-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58e22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e22-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="58e22-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58e22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e22-116">Not supported.</span></span>|
|<span data-ttu-id="58e22-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58e22-117">Application</span></span>|<span data-ttu-id="58e22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e22-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58e22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="58e22-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58e22-120">Request headers</span></span>
|<span data-ttu-id="58e22-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58e22-121">Header</span></span>|<span data-ttu-id="58e22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58e22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58e22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e22-123">Authorization</span></span>|<span data-ttu-id="58e22-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58e22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58e22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58e22-125">Accept</span></span>|<span data-ttu-id="58e22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58e22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58e22-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58e22-127">Request body</span></span>
<span data-ttu-id="58e22-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58e22-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="58e22-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="58e22-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="58e22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58e22-130">Property</span></span>|<span data-ttu-id="58e22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58e22-131">Type</span></span>|<span data-ttu-id="58e22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58e22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58e22-133">version</span><span class="sxs-lookup"><span data-stu-id="58e22-133">version</span></span>|<span data-ttu-id="58e22-134">String</span><span class="sxs-lookup"><span data-stu-id="58e22-134">String</span></span>|<span data-ttu-id="58e22-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="58e22-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="58e22-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e22-136">Response</span></span>
<span data-ttu-id="58e22-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58e22-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e22-138">Пример</span><span class="sxs-lookup"><span data-stu-id="58e22-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="58e22-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e22-139">Request</span></span>
<span data-ttu-id="58e22-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58e22-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="58e22-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e22-141">Response</span></span>
<span data-ttu-id="58e22-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58e22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```



