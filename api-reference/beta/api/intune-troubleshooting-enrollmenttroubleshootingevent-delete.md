---
title: Удаление объекта enrollmentTroubleshootingEvent
description: Удаляет объект enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c9c9055c2b3e64c37729859dbc26d71f26c9fa3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816207"
---
# <a name="delete-enrollmenttroubleshootingevent"></a><span data-ttu-id="46bbc-103">Удаление объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="46bbc-103">Delete enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="46bbc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46bbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46bbc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46bbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46bbc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46bbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46bbc-107">Удаляет объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="46bbc-107">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46bbc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46bbc-108">Prerequisites</span></span>
<span data-ttu-id="46bbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46bbc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46bbc-111">Permission type</span></span>|<span data-ttu-id="46bbc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46bbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46bbc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46bbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46bbc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46bbc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="46bbc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46bbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46bbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46bbc-116">Not supported.</span></span>|
|<span data-ttu-id="46bbc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46bbc-117">Application</span></span>|<span data-ttu-id="46bbc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46bbc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46bbc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46bbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="46bbc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46bbc-120">Request headers</span></span>
|<span data-ttu-id="46bbc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46bbc-121">Header</span></span>|<span data-ttu-id="46bbc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46bbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46bbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46bbc-123">Authorization</span></span>|<span data-ttu-id="46bbc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46bbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46bbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46bbc-125">Accept</span></span>|<span data-ttu-id="46bbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46bbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46bbc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46bbc-127">Request body</span></span>
<span data-ttu-id="46bbc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46bbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46bbc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="46bbc-129">Response</span></span>
<span data-ttu-id="46bbc-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46bbc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46bbc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="46bbc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="46bbc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46bbc-132">Request</span></span>
<span data-ttu-id="46bbc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46bbc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="46bbc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="46bbc-134">Response</span></span>
<span data-ttu-id="46bbc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46bbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





