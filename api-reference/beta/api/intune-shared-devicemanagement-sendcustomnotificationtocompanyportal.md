---
title: Действие sendCustomNotificationToCompanyPortal
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b5a3e4acedb95fe1092a6ef9eaacc2978fedcd9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851165"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="20318-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="20318-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="20318-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20318-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20318-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20318-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20318-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20318-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20318-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20318-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20318-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="20318-108">Prerequisites</span></span>
<span data-ttu-id="20318-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20318-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20318-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20318-111">Permission type</span></span>|<span data-ttu-id="20318-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20318-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20318-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20318-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="20318-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="20318-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="20318-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20318-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20318-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20318-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20318-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20318-117">Not supported.</span></span>|
|<span data-ttu-id="20318-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20318-118">Application</span></span>|<span data-ttu-id="20318-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20318-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20318-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20318-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="20318-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20318-121">Request headers</span></span>
|<span data-ttu-id="20318-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20318-122">Header</span></span>|<span data-ttu-id="20318-123">Значение</span><span class="sxs-lookup"><span data-stu-id="20318-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20318-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20318-124">Authorization</span></span>|<span data-ttu-id="20318-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20318-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20318-126">Accept</span><span class="sxs-lookup"><span data-stu-id="20318-126">Accept</span></span>|<span data-ttu-id="20318-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20318-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20318-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20318-128">Request body</span></span>
<span data-ttu-id="20318-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20318-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="20318-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="20318-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="20318-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="20318-131">Property</span></span>|<span data-ttu-id="20318-132">Тип</span><span class="sxs-lookup"><span data-stu-id="20318-132">Type</span></span>|<span data-ttu-id="20318-133">Описание</span><span class="sxs-lookup"><span data-stu-id="20318-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20318-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="20318-134">notificationTitle</span></span>|<span data-ttu-id="20318-135">Строка</span><span class="sxs-lookup"><span data-stu-id="20318-135">String</span></span>|<span data-ttu-id="20318-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20318-136">Not yet documented</span></span>|
|<span data-ttu-id="20318-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="20318-137">notificationBody</span></span>|<span data-ttu-id="20318-138">Строка</span><span class="sxs-lookup"><span data-stu-id="20318-138">String</span></span>|<span data-ttu-id="20318-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20318-139">Not yet documented</span></span>|
|<span data-ttu-id="20318-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="20318-140">groupsToNotify</span></span>|<span data-ttu-id="20318-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20318-141">String collection</span></span>|<span data-ttu-id="20318-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="20318-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="20318-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="20318-143">Response</span></span>
<span data-ttu-id="20318-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="20318-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20318-145">Пример</span><span class="sxs-lookup"><span data-stu-id="20318-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="20318-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="20318-146">Request</span></span>
<span data-ttu-id="20318-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20318-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20318-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="20318-148">Response</span></span>
<span data-ttu-id="20318-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20318-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






