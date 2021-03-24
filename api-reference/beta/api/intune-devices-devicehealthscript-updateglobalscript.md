---
title: updateGlobalScript action
description: Обновление скрипта здоровья несвободных устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c943a7b22523934808d9d3382ea929a024783502
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127097"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="28142-103">updateGlobalScript action</span><span class="sxs-lookup"><span data-stu-id="28142-103">updateGlobalScript action</span></span>

<span data-ttu-id="28142-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28142-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28142-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28142-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28142-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28142-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28142-107">Обновление скрипта здоровья несвободных устройств</span><span class="sxs-lookup"><span data-stu-id="28142-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28142-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28142-108">Prerequisites</span></span>
<span data-ttu-id="28142-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28142-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28142-111">Permission type</span></span>|<span data-ttu-id="28142-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28142-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28142-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28142-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28142-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28142-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28142-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28142-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28142-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28142-116">Not supported.</span></span>|
|<span data-ttu-id="28142-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28142-117">Application</span></span>|<span data-ttu-id="28142-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28142-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28142-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28142-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="28142-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28142-120">Request headers</span></span>
|<span data-ttu-id="28142-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28142-121">Header</span></span>|<span data-ttu-id="28142-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28142-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28142-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28142-123">Authorization</span></span>|<span data-ttu-id="28142-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28142-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28142-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28142-125">Accept</span></span>|<span data-ttu-id="28142-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28142-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28142-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28142-127">Request body</span></span>
<span data-ttu-id="28142-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28142-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="28142-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="28142-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="28142-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28142-130">Property</span></span>|<span data-ttu-id="28142-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28142-131">Type</span></span>|<span data-ttu-id="28142-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28142-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28142-133">version</span><span class="sxs-lookup"><span data-stu-id="28142-133">version</span></span>|<span data-ttu-id="28142-134">String</span><span class="sxs-lookup"><span data-stu-id="28142-134">String</span></span>|<span data-ttu-id="28142-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="28142-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="28142-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="28142-136">Response</span></span>
<span data-ttu-id="28142-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28142-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28142-138">Пример</span><span class="sxs-lookup"><span data-stu-id="28142-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="28142-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="28142-139">Request</span></span>
<span data-ttu-id="28142-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28142-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="28142-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="28142-141">Response</span></span>
<span data-ttu-id="28142-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28142-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```




