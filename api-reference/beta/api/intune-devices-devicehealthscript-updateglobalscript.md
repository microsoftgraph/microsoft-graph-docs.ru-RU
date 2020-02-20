---
title: действие Упдатеглобалскрипт
description: Обновление сценария работоспособности собственного устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 366fdcb5f19d6e50dfa5936c45c984cddbfb6d6d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162185"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="c603e-103">действие Упдатеглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="c603e-103">updateGlobalScript action</span></span>

> <span data-ttu-id="c603e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c603e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c603e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c603e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c603e-106">Обновление сценария работоспособности собственного устройства</span><span class="sxs-lookup"><span data-stu-id="c603e-106">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c603e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c603e-107">Prerequisites</span></span>
<span data-ttu-id="c603e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c603e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c603e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c603e-110">Permission type</span></span>|<span data-ttu-id="c603e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c603e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c603e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c603e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c603e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c603e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c603e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c603e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c603e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c603e-115">Not supported.</span></span>|
|<span data-ttu-id="c603e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c603e-116">Application</span></span>|<span data-ttu-id="c603e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c603e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c603e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c603e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="c603e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c603e-119">Request headers</span></span>
|<span data-ttu-id="c603e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c603e-120">Header</span></span>|<span data-ttu-id="c603e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c603e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c603e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c603e-122">Authorization</span></span>|<span data-ttu-id="c603e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c603e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c603e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c603e-124">Accept</span></span>|<span data-ttu-id="c603e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c603e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c603e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c603e-126">Request body</span></span>
<span data-ttu-id="c603e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c603e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c603e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c603e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c603e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c603e-129">Property</span></span>|<span data-ttu-id="c603e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c603e-130">Type</span></span>|<span data-ttu-id="c603e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c603e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c603e-132">version</span><span class="sxs-lookup"><span data-stu-id="c603e-132">version</span></span>|<span data-ttu-id="c603e-133">String</span><span class="sxs-lookup"><span data-stu-id="c603e-133">String</span></span>|<span data-ttu-id="c603e-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c603e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c603e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c603e-135">Response</span></span>
<span data-ttu-id="c603e-136">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c603e-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c603e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c603e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c603e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c603e-138">Request</span></span>
<span data-ttu-id="c603e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c603e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="c603e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c603e-140">Response</span></span>
<span data-ttu-id="c603e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c603e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```





