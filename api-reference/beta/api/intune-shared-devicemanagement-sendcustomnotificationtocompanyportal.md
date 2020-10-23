---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a1bf5044c48c1ca74ffcca883029f48f7c73acb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692831"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="2ae62-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2ae62-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="2ae62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ae62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ae62-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ae62-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ae62-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae62-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ae62-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ae62-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ae62-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2ae62-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ae62-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ae62-109">Prerequisites</span></span>
<span data-ttu-id="2ae62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ae62-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae62-112">Permission type</span></span>|<span data-ttu-id="2ae62-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ae62-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ae62-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ae62-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2ae62-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2ae62-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2ae62-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae62-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ae62-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ae62-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ae62-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae62-118">Not supported.</span></span>|
|<span data-ttu-id="2ae62-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ae62-119">Application</span></span>||
| <span data-ttu-id="2ae62-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2ae62-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2ae62-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae62-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="2ae62-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ae62-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="2ae62-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ae62-123">Request headers</span></span>
|<span data-ttu-id="2ae62-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ae62-124">Header</span></span>|<span data-ttu-id="2ae62-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2ae62-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ae62-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ae62-126">Authorization</span></span>|<span data-ttu-id="2ae62-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ae62-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ae62-128">Accept</span><span class="sxs-lookup"><span data-stu-id="2ae62-128">Accept</span></span>|<span data-ttu-id="2ae62-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2ae62-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ae62-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ae62-130">Request body</span></span>
<span data-ttu-id="2ae62-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ae62-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2ae62-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2ae62-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2ae62-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ae62-133">Property</span></span>|<span data-ttu-id="2ae62-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2ae62-134">Type</span></span>|<span data-ttu-id="2ae62-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae62-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ae62-136">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="2ae62-136">notificationTitle</span></span>|<span data-ttu-id="2ae62-137">String</span><span class="sxs-lookup"><span data-stu-id="2ae62-137">String</span></span>|<span data-ttu-id="2ae62-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2ae62-138">Not yet documented</span></span>|
|<span data-ttu-id="2ae62-139">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="2ae62-139">notificationBody</span></span>|<span data-ttu-id="2ae62-140">String</span><span class="sxs-lookup"><span data-stu-id="2ae62-140">String</span></span>|<span data-ttu-id="2ae62-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2ae62-141">Not yet documented</span></span>|
|<span data-ttu-id="2ae62-142">граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="2ae62-142">groupsToNotify</span></span>|<span data-ttu-id="2ae62-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ae62-143">String collection</span></span>|<span data-ttu-id="2ae62-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2ae62-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2ae62-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ae62-145">Response</span></span>
<span data-ttu-id="2ae62-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ae62-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ae62-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2ae62-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ae62-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ae62-148">Request</span></span>
<span data-ttu-id="2ae62-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ae62-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ae62-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ae62-150">Response</span></span>
<span data-ttu-id="2ae62-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ae62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```














