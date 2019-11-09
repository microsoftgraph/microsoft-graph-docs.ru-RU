---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b72f97ad6cb579fd907429cee0e5f73d4663fe84
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086041"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="df7cf-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="df7cf-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="df7cf-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="df7cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df7cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df7cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df7cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df7cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df7cf-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="df7cf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df7cf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="df7cf-108">Prerequisites</span></span>
<span data-ttu-id="df7cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df7cf-111">Permission type</span></span>|<span data-ttu-id="df7cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df7cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df7cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df7cf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df7cf-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="df7cf-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="df7cf-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7cf-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="df7cf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df7cf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df7cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df7cf-117">Not supported.</span></span>|
|<span data-ttu-id="df7cf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df7cf-118">Application</span></span>||
| <span data-ttu-id="df7cf-119">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="df7cf-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="df7cf-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7cf-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="df7cf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df7cf-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="df7cf-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df7cf-122">Request headers</span></span>
|<span data-ttu-id="df7cf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df7cf-123">Header</span></span>|<span data-ttu-id="df7cf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="df7cf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df7cf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df7cf-125">Authorization</span></span>|<span data-ttu-id="df7cf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df7cf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df7cf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="df7cf-127">Accept</span></span>|<span data-ttu-id="df7cf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="df7cf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7cf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df7cf-129">Request body</span></span>
<span data-ttu-id="df7cf-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df7cf-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df7cf-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="df7cf-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df7cf-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="df7cf-132">Property</span></span>|<span data-ttu-id="df7cf-133">Тип</span><span class="sxs-lookup"><span data-stu-id="df7cf-133">Type</span></span>|<span data-ttu-id="df7cf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="df7cf-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df7cf-135">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="df7cf-135">notificationTitle</span></span>|<span data-ttu-id="df7cf-136">String</span><span class="sxs-lookup"><span data-stu-id="df7cf-136">String</span></span>|<span data-ttu-id="df7cf-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="df7cf-137">Not yet documented</span></span>|
|<span data-ttu-id="df7cf-138">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="df7cf-138">notificationBody</span></span>|<span data-ttu-id="df7cf-139">String</span><span class="sxs-lookup"><span data-stu-id="df7cf-139">String</span></span>|<span data-ttu-id="df7cf-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="df7cf-140">Not yet documented</span></span>|
|<span data-ttu-id="df7cf-141">граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="df7cf-141">groupsToNotify</span></span>|<span data-ttu-id="df7cf-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="df7cf-142">String collection</span></span>|<span data-ttu-id="df7cf-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df7cf-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df7cf-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="df7cf-144">Response</span></span>
<span data-ttu-id="df7cf-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df7cf-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df7cf-146">Пример</span><span class="sxs-lookup"><span data-stu-id="df7cf-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="df7cf-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="df7cf-147">Request</span></span>
<span data-ttu-id="df7cf-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df7cf-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df7cf-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="df7cf-149">Response</span></span>
<span data-ttu-id="df7cf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df7cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```















