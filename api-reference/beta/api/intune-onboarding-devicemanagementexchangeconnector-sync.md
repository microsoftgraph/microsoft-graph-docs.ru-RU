---
title: Действие sync
description: Н/Д
author: tfitzmac
ms.openlocfilehash: fb9fa6aa7cd2e33ba75922b32dada12d5e80b470
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330781"
---
# <a name="sync-action"></a><span data-ttu-id="880a8-103">Действие sync</span><span class="sxs-lookup"><span data-stu-id="880a8-103">sync action</span></span>

> <span data-ttu-id="880a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="880a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="880a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="880a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="880a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="880a8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="880a8-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="880a8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="880a8-108">Prerequisites</span></span>
<span data-ttu-id="880a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="880a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="880a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="880a8-111">Permission type</span></span>|<span data-ttu-id="880a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="880a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="880a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="880a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="880a8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="880a8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="880a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="880a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="880a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880a8-116">Not supported.</span></span>|
|<span data-ttu-id="880a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="880a8-117">Application</span></span>|<span data-ttu-id="880a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="880a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="880a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="880a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="880a8-120">Request headers</span></span>
|<span data-ttu-id="880a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="880a8-121">Header</span></span>|<span data-ttu-id="880a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="880a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="880a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="880a8-123">Authorization</span></span>|<span data-ttu-id="880a8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="880a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="880a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="880a8-125">Accept</span></span>|<span data-ttu-id="880a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="880a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="880a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="880a8-127">Request body</span></span>
<span data-ttu-id="880a8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="880a8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="880a8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="880a8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="880a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="880a8-130">Property</span></span>|<span data-ttu-id="880a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="880a8-131">Type</span></span>|<span data-ttu-id="880a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="880a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880a8-133">syncType</span><span class="sxs-lookup"><span data-stu-id="880a8-133">syncType</span></span>|[<span data-ttu-id="880a8-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="880a8-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="880a8-135">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="880a8-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="880a8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="880a8-136">Response</span></span>
<span data-ttu-id="880a8-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="880a8-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="880a8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="880a8-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="880a8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="880a8-139">Request</span></span>
<span data-ttu-id="880a8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="880a8-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="880a8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="880a8-141">Response</span></span>
<span data-ttu-id="880a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="880a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





