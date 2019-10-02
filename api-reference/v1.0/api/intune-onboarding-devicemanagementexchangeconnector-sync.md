---
title: Действие sync
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7b3ced55f3a9ce94af3812538411aa0f283c18e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362430"
---
# <a name="sync-action"></a><span data-ttu-id="fc077-103">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="fc077-103">sync action</span></span>

> <span data-ttu-id="fc077-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc077-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc077-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fc077-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc077-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc077-106">Prerequisites</span></span>
<span data-ttu-id="fc077-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc077-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc077-109">Permission type</span></span>|<span data-ttu-id="fc077-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc077-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc077-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc077-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc077-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc077-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc077-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc077-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc077-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc077-114">Not supported.</span></span>|
|<span data-ttu-id="fc077-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc077-115">Application</span></span>|<span data-ttu-id="fc077-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc077-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc077-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc077-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="fc077-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc077-118">Request headers</span></span>
|<span data-ttu-id="fc077-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc077-119">Header</span></span>|<span data-ttu-id="fc077-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fc077-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc077-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc077-121">Authorization</span></span>|<span data-ttu-id="fc077-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc077-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc077-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fc077-123">Accept</span></span>|<span data-ttu-id="fc077-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc077-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc077-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc077-125">Request body</span></span>
<span data-ttu-id="fc077-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc077-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fc077-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fc077-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fc077-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc077-128">Property</span></span>|<span data-ttu-id="fc077-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fc077-129">Type</span></span>|<span data-ttu-id="fc077-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fc077-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc077-131">syncType</span><span class="sxs-lookup"><span data-stu-id="fc077-131">syncType</span></span>|[<span data-ttu-id="fc077-132">девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="fc077-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="fc077-133">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="fc077-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="fc077-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc077-134">Response</span></span>
<span data-ttu-id="fc077-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fc077-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fc077-136">Пример</span><span class="sxs-lookup"><span data-stu-id="fc077-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc077-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc077-137">Request</span></span>
<span data-ttu-id="fc077-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc077-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="fc077-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc077-139">Response</span></span>
<span data-ttu-id="fc077-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc077-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




