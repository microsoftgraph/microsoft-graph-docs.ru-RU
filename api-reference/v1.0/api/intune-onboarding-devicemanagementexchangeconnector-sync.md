---
title: Действие sync
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98e2c1671b7fde9450b18ca3bd12537450d02416
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988478"
---
# <a name="sync-action"></a><span data-ttu-id="80b80-103">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="80b80-103">sync action</span></span>

> <span data-ttu-id="80b80-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80b80-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80b80-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="80b80-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80b80-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="80b80-106">Prerequisites</span></span>
<span data-ttu-id="80b80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80b80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80b80-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80b80-109">Permission type</span></span>|<span data-ttu-id="80b80-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80b80-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80b80-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80b80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80b80-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b80-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80b80-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80b80-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80b80-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b80-114">Not supported.</span></span>|
|<span data-ttu-id="80b80-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80b80-115">Application</span></span>|<span data-ttu-id="80b80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80b80-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80b80-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80b80-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="80b80-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80b80-118">Request headers</span></span>
|<span data-ttu-id="80b80-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80b80-119">Header</span></span>|<span data-ttu-id="80b80-120">Значение</span><span class="sxs-lookup"><span data-stu-id="80b80-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80b80-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80b80-121">Authorization</span></span>|<span data-ttu-id="80b80-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80b80-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80b80-123">Accept</span><span class="sxs-lookup"><span data-stu-id="80b80-123">Accept</span></span>|<span data-ttu-id="80b80-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80b80-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80b80-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80b80-125">Request body</span></span>
<span data-ttu-id="80b80-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80b80-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="80b80-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="80b80-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="80b80-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="80b80-128">Property</span></span>|<span data-ttu-id="80b80-129">Тип</span><span class="sxs-lookup"><span data-stu-id="80b80-129">Type</span></span>|<span data-ttu-id="80b80-130">Описание</span><span class="sxs-lookup"><span data-stu-id="80b80-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80b80-131">syncType</span><span class="sxs-lookup"><span data-stu-id="80b80-131">syncType</span></span>|[<span data-ttu-id="80b80-132">Девицеманажементексчанжеконнекторсинктипе</span><span class="sxs-lookup"><span data-stu-id="80b80-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="80b80-133">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="80b80-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="80b80-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b80-134">Response</span></span>
<span data-ttu-id="80b80-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80b80-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80b80-136">Пример</span><span class="sxs-lookup"><span data-stu-id="80b80-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="80b80-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="80b80-137">Request</span></span>
<span data-ttu-id="80b80-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80b80-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="80b80-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="80b80-139">Response</span></span>
<span data-ttu-id="80b80-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80b80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



