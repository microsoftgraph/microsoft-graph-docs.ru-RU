---
title: Действие sync
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ec694deb39a821d42ec5defb4322844332a3bdf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827456"
---
# <a name="sync-action"></a><span data-ttu-id="4e842-103">Действие sync</span><span class="sxs-lookup"><span data-stu-id="4e842-103">sync action</span></span>

> <span data-ttu-id="4e842-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e842-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e842-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e842-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e842-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e842-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e842-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e842-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4e842-108">Prerequisites</span></span>
<span data-ttu-id="4e842-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e842-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e842-111">Permission type</span></span>|<span data-ttu-id="4e842-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e842-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e842-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e842-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e842-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4e842-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e842-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e842-116">Not supported.</span></span>|
|<span data-ttu-id="4e842-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e842-117">Application</span></span>|<span data-ttu-id="4e842-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e842-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e842-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="4e842-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e842-120">Request headers</span></span>
|<span data-ttu-id="4e842-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e842-121">Header</span></span>|<span data-ttu-id="4e842-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e842-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e842-123">Authorization</span></span>|<span data-ttu-id="4e842-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e842-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e842-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e842-125">Accept</span></span>|<span data-ttu-id="4e842-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e842-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e842-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e842-127">Request body</span></span>
<span data-ttu-id="4e842-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e842-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e842-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e842-129">Response</span></span>
<span data-ttu-id="4e842-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e842-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e842-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4e842-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e842-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e842-132">Request</span></span>
<span data-ttu-id="4e842-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e842-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="4e842-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e842-134">Response</span></span>
<span data-ttu-id="4e842-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e842-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





