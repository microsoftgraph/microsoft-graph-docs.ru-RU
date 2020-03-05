---
title: действие Жетглобалскрипсигхеставаилаблеверсион
description: Обновление сценария работоспособности собственного устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9ee758cb448051499d1613feb0a816f4c35909a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469687"
---
# <a name="getglobalscripthighestavailableversion-action"></a><span data-ttu-id="9a108-103">действие Жетглобалскрипсигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="9a108-103">getGlobalScriptHighestAvailableVersion action</span></span>

<span data-ttu-id="9a108-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a108-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a108-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a108-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a108-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a108-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a108-107">Обновление сценария работоспособности собственного устройства</span><span class="sxs-lookup"><span data-stu-id="9a108-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a108-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a108-108">Prerequisites</span></span>
<span data-ttu-id="9a108-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a108-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a108-111">Permission type</span></span>|<span data-ttu-id="9a108-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a108-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a108-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a108-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a108-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a108-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9a108-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a108-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a108-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a108-116">Not supported.</span></span>|
|<span data-ttu-id="9a108-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a108-117">Application</span></span>|<span data-ttu-id="9a108-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a108-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a108-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a108-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

## <a name="request-headers"></a><span data-ttu-id="9a108-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a108-120">Request headers</span></span>
|<span data-ttu-id="9a108-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a108-121">Header</span></span>|<span data-ttu-id="9a108-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a108-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a108-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a108-123">Authorization</span></span>|<span data-ttu-id="9a108-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a108-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a108-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a108-125">Accept</span></span>|<span data-ttu-id="9a108-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a108-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a108-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a108-127">Request body</span></span>
<span data-ttu-id="9a108-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a108-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a108-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a108-129">Response</span></span>
<span data-ttu-id="9a108-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a108-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a108-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9a108-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a108-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a108-132">Request</span></span>
<span data-ttu-id="9a108-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a108-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

### <a name="response"></a><span data-ttu-id="9a108-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a108-134">Response</span></span>
<span data-ttu-id="9a108-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a108-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 68

{
  "value": "Get Global Script Highest Available Version value"
}
```





