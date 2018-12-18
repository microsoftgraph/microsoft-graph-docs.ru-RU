---
title: Действие sendCustomNotificationToCompanyPortal
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 549aff553416e6e8c5fa03382b7a4e513a4ede83
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305245"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="84815-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="84815-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="84815-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84815-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84815-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84815-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84815-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84815-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84815-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="84815-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84815-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="84815-108">Prerequisites</span></span>
<span data-ttu-id="84815-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84815-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84815-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84815-111">Permission type</span></span>|<span data-ttu-id="84815-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84815-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84815-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84815-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84815-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84815-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84815-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84815-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84815-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84815-116">Not supported.</span></span>|
|<span data-ttu-id="84815-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84815-117">Application</span></span>|<span data-ttu-id="84815-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84815-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84815-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84815-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="84815-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84815-120">Request headers</span></span>
|<span data-ttu-id="84815-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84815-121">Header</span></span>|<span data-ttu-id="84815-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84815-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84815-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84815-123">Authorization</span></span>|<span data-ttu-id="84815-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84815-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84815-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84815-125">Accept</span></span>|<span data-ttu-id="84815-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84815-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84815-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84815-127">Request body</span></span>
<span data-ttu-id="84815-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84815-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="84815-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="84815-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="84815-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84815-130">Property</span></span>|<span data-ttu-id="84815-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84815-131">Type</span></span>|<span data-ttu-id="84815-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84815-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84815-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="84815-133">notificationTitle</span></span>|<span data-ttu-id="84815-134">Строка</span><span class="sxs-lookup"><span data-stu-id="84815-134">String</span></span>|<span data-ttu-id="84815-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="84815-135">Not yet documented</span></span>|
|<span data-ttu-id="84815-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="84815-136">notificationBody</span></span>|<span data-ttu-id="84815-137">Строка</span><span class="sxs-lookup"><span data-stu-id="84815-137">String</span></span>|<span data-ttu-id="84815-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="84815-138">Not yet documented</span></span>|
|<span data-ttu-id="84815-139">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="84815-139">groupsToNotify</span></span>|<span data-ttu-id="84815-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="84815-140">String collection</span></span>|<span data-ttu-id="84815-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="84815-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84815-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="84815-142">Response</span></span>
<span data-ttu-id="84815-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="84815-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84815-144">Пример</span><span class="sxs-lookup"><span data-stu-id="84815-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="84815-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="84815-145">Request</span></span>
<span data-ttu-id="84815-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84815-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84815-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="84815-147">Response</span></span>
<span data-ttu-id="84815-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84815-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





