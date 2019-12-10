---
title: Действие sync
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c496b952c83f25e60f7a4f4c78a6d55154dc8ca8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941745"
---
# <a name="sync-action"></a><span data-ttu-id="cd9c9-103">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="cd9c9-103">sync action</span></span>

> <span data-ttu-id="cd9c9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd9c9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd9c9-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9c9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd9c9-107">Prerequisites</span></span>
<span data-ttu-id="cd9c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd9c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9c9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9c9-110">Permission type</span></span>|<span data-ttu-id="cd9c9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9c9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd9c9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9c9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd9c9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-115">Not supported.</span></span>|
|<span data-ttu-id="cd9c9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd9c9-116">Application</span></span>|<span data-ttu-id="cd9c9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9c9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9c9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd9c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="cd9c9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd9c9-119">Request headers</span></span>
|<span data-ttu-id="cd9c9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd9c9-120">Header</span></span>|<span data-ttu-id="cd9c9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd9c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9c9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd9c9-122">Authorization</span></span>|<span data-ttu-id="cd9c9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9c9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd9c9-124">Accept</span></span>|<span data-ttu-id="cd9c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9c9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd9c9-126">Request body</span></span>
<span data-ttu-id="cd9c9-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cd9c9-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cd9c9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd9c9-129">Property</span></span>|<span data-ttu-id="cd9c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd9c9-130">Type</span></span>|<span data-ttu-id="cd9c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd9c9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9c9-132">syncType</span><span class="sxs-lookup"><span data-stu-id="cd9c9-132">syncType</span></span>|[<span data-ttu-id="cd9c9-133">девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="cd9c9-133">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="cd9c9-134">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="cd9c9-134">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="cd9c9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9c9-135">Response</span></span>
<span data-ttu-id="cd9c9-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd9c9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cd9c9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9c9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9c9-138">Request</span></span>
<span data-ttu-id="cd9c9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="cd9c9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9c9-140">Response</span></span>
<span data-ttu-id="cd9c9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





