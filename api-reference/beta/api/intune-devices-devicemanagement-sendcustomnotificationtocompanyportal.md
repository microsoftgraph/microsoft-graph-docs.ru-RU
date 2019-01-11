---
title: Действие sendCustomNotificationToCompanyPortal
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9ea1cb5a2bcdf18c38dfc144d57e7ee77a5d6fd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863331"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="42068-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="42068-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="42068-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42068-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42068-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42068-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42068-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="42068-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42068-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42068-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42068-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="42068-108">Prerequisites</span></span>
<span data-ttu-id="42068-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42068-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42068-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42068-111">Permission type</span></span>|<span data-ttu-id="42068-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42068-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42068-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42068-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42068-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42068-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42068-116">Not supported.</span></span>|
|<span data-ttu-id="42068-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42068-117">Application</span></span>|<span data-ttu-id="42068-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42068-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42068-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="42068-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42068-120">Request headers</span></span>
|<span data-ttu-id="42068-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42068-121">Header</span></span>|<span data-ttu-id="42068-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42068-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42068-123">Authorization</span></span>|<span data-ttu-id="42068-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42068-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42068-125">Accept</span></span>|<span data-ttu-id="42068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42068-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42068-127">Request body</span></span>
<span data-ttu-id="42068-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42068-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42068-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="42068-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42068-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42068-130">Property</span></span>|<span data-ttu-id="42068-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42068-131">Type</span></span>|<span data-ttu-id="42068-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42068-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42068-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="42068-133">notificationTitle</span></span>|<span data-ttu-id="42068-134">Строка</span><span class="sxs-lookup"><span data-stu-id="42068-134">String</span></span>|<span data-ttu-id="42068-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42068-135">Not yet documented</span></span>|
|<span data-ttu-id="42068-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="42068-136">notificationBody</span></span>|<span data-ttu-id="42068-137">Строка</span><span class="sxs-lookup"><span data-stu-id="42068-137">String</span></span>|<span data-ttu-id="42068-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42068-138">Not yet documented</span></span>|
|<span data-ttu-id="42068-139">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="42068-139">groupsToNotify</span></span>|<span data-ttu-id="42068-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42068-140">String collection</span></span>|<span data-ttu-id="42068-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42068-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42068-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="42068-142">Response</span></span>
<span data-ttu-id="42068-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42068-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42068-144">Пример</span><span class="sxs-lookup"><span data-stu-id="42068-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="42068-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="42068-145">Request</span></span>
<span data-ttu-id="42068-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42068-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 164

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "groupsToNotify": [
    "Groups To Notify value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="42068-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="42068-147">Response</span></span>
<span data-ttu-id="42068-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42068-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





