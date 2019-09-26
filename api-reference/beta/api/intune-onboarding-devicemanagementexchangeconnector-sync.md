---
title: Действие sync
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f896f49da70a48ef5a628af4e8abf01c05da762f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190772"
---
# <a name="sync-action"></a><span data-ttu-id="1c851-103">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="1c851-103">sync action</span></span>

> <span data-ttu-id="1c851-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c851-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c851-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c851-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c851-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1c851-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c851-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1c851-107">Prerequisites</span></span>
<span data-ttu-id="1c851-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c851-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c851-110">Permission type</span></span>|<span data-ttu-id="1c851-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c851-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c851-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c851-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c851-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c851-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c851-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c851-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c851-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c851-115">Not supported.</span></span>|
|<span data-ttu-id="1c851-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c851-116">Application</span></span>|<span data-ttu-id="1c851-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c851-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c851-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c851-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="1c851-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c851-119">Request headers</span></span>
|<span data-ttu-id="1c851-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c851-120">Header</span></span>|<span data-ttu-id="1c851-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1c851-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c851-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c851-122">Authorization</span></span>|<span data-ttu-id="1c851-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c851-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c851-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1c851-124">Accept</span></span>|<span data-ttu-id="1c851-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c851-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c851-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c851-126">Request body</span></span>
<span data-ttu-id="1c851-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c851-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c851-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="1c851-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c851-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c851-129">Property</span></span>|<span data-ttu-id="1c851-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c851-130">Type</span></span>|<span data-ttu-id="1c851-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c851-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c851-132">syncType</span><span class="sxs-lookup"><span data-stu-id="1c851-132">syncType</span></span>|[<span data-ttu-id="1c851-133">девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="1c851-133">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="1c851-134">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="1c851-134">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="1c851-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c851-135">Response</span></span>
<span data-ttu-id="1c851-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c851-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c851-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1c851-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c851-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c851-138">Request</span></span>
<span data-ttu-id="1c851-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c851-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="1c851-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c851-140">Response</span></span>
<span data-ttu-id="1c851-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c851-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




