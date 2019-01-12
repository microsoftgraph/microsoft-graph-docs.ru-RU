---
title: Действие sync
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f850569c74bee27df9c5d1d0a4eb41630cc1265b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957146"
---
# <a name="sync-action"></a><span data-ttu-id="841c4-103">Действие sync</span><span class="sxs-lookup"><span data-stu-id="841c4-103">sync action</span></span>

> <span data-ttu-id="841c4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="841c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="841c4-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="841c4-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="841c4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="841c4-106">Prerequisites</span></span>
<span data-ttu-id="841c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="841c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="841c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="841c4-109">Permission type</span></span>|<span data-ttu-id="841c4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="841c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="841c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="841c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="841c4-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="841c4-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="841c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="841c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="841c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="841c4-114">Not supported.</span></span>|
|<span data-ttu-id="841c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="841c4-115">Application</span></span>|<span data-ttu-id="841c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="841c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="841c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="841c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="841c4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="841c4-118">Request headers</span></span>
|<span data-ttu-id="841c4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="841c4-119">Header</span></span>|<span data-ttu-id="841c4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="841c4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="841c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="841c4-121">Authorization</span></span>|<span data-ttu-id="841c4-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="841c4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="841c4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="841c4-123">Accept</span></span>|<span data-ttu-id="841c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="841c4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="841c4-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="841c4-125">Request body</span></span>
<span data-ttu-id="841c4-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="841c4-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="841c4-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="841c4-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="841c4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="841c4-128">Property</span></span>|<span data-ttu-id="841c4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="841c4-129">Type</span></span>|<span data-ttu-id="841c4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="841c4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="841c4-131">syncType</span><span class="sxs-lookup"><span data-stu-id="841c4-131">syncType</span></span>|[<span data-ttu-id="841c4-132">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="841c4-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="841c4-133">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="841c4-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="841c4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="841c4-134">Response</span></span>
<span data-ttu-id="841c4-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="841c4-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="841c4-136">Пример</span><span class="sxs-lookup"><span data-stu-id="841c4-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="841c4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="841c4-137">Request</span></span>
<span data-ttu-id="841c4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="841c4-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="841c4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="841c4-139">Response</span></span>
<span data-ttu-id="841c4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="841c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



