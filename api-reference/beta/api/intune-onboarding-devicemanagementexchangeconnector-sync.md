---
title: Действие sync
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a86be438ddadfce305690eb36e07372252161a6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462154"
---
# <a name="sync-action"></a><span data-ttu-id="955b2-103">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="955b2-103">sync action</span></span>

<span data-ttu-id="955b2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="955b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="955b2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="955b2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="955b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="955b2-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="955b2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="955b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="955b2-108">Prerequisites</span></span>
<span data-ttu-id="955b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="955b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="955b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="955b2-111">Permission type</span></span>|<span data-ttu-id="955b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="955b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="955b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="955b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="955b2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="955b2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="955b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="955b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="955b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955b2-116">Not supported.</span></span>|
|<span data-ttu-id="955b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="955b2-117">Application</span></span>|<span data-ttu-id="955b2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="955b2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="955b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="955b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="955b2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="955b2-120">Request headers</span></span>
|<span data-ttu-id="955b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="955b2-121">Header</span></span>|<span data-ttu-id="955b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="955b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="955b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="955b2-123">Authorization</span></span>|<span data-ttu-id="955b2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="955b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="955b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="955b2-125">Accept</span></span>|<span data-ttu-id="955b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="955b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="955b2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="955b2-127">Request body</span></span>
<span data-ttu-id="955b2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955b2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="955b2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="955b2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="955b2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="955b2-130">Property</span></span>|<span data-ttu-id="955b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="955b2-131">Type</span></span>|<span data-ttu-id="955b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="955b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955b2-133">syncType</span><span class="sxs-lookup"><span data-stu-id="955b2-133">syncType</span></span>|[<span data-ttu-id="955b2-134">девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="955b2-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="955b2-135">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="955b2-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="955b2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="955b2-136">Response</span></span>
<span data-ttu-id="955b2-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="955b2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="955b2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="955b2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="955b2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="955b2-139">Request</span></span>
<span data-ttu-id="955b2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="955b2-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="955b2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="955b2-141">Response</span></span>
<span data-ttu-id="955b2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="955b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





