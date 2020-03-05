---
title: Удаление Девицехеалсскрипт
description: Удаляет объект Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26ab428a34aff902760093c1b777386009624087
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469729"
---
# <a name="delete-devicehealthscript"></a><span data-ttu-id="63c94-103">Удаление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="63c94-103">Delete deviceHealthScript</span></span>

<span data-ttu-id="63c94-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="63c94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63c94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63c94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63c94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63c94-107">Удаляет объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="63c94-107">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63c94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63c94-108">Prerequisites</span></span>
<span data-ttu-id="63c94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63c94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63c94-111">Permission type</span></span>|<span data-ttu-id="63c94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63c94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63c94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63c94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63c94-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63c94-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63c94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63c94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63c94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c94-116">Not supported.</span></span>|
|<span data-ttu-id="63c94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63c94-117">Application</span></span>|<span data-ttu-id="63c94-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63c94-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63c94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63c94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="63c94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63c94-120">Request headers</span></span>
|<span data-ttu-id="63c94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63c94-121">Header</span></span>|<span data-ttu-id="63c94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63c94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63c94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63c94-123">Authorization</span></span>|<span data-ttu-id="63c94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63c94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63c94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63c94-125">Accept</span></span>|<span data-ttu-id="63c94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63c94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63c94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63c94-127">Request body</span></span>
<span data-ttu-id="63c94-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63c94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63c94-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c94-129">Response</span></span>
<span data-ttu-id="63c94-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63c94-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63c94-131">Пример</span><span class="sxs-lookup"><span data-stu-id="63c94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63c94-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="63c94-132">Request</span></span>
<span data-ttu-id="63c94-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63c94-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

### <a name="response"></a><span data-ttu-id="63c94-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c94-134">Response</span></span>
<span data-ttu-id="63c94-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63c94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





