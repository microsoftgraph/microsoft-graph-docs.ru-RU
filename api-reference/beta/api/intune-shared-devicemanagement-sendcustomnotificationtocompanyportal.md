---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf850c6bb6866c0f71d6da869e63b5d73f6288d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390061"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="35cd1-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="35cd1-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="35cd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35cd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35cd1-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35cd1-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35cd1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35cd1-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35cd1-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35cd1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35cd1-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35cd1-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35cd1-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="35cd1-109">Prerequisites</span></span>
<span data-ttu-id="35cd1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35cd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35cd1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35cd1-112">Permission type</span></span>|<span data-ttu-id="35cd1-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35cd1-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35cd1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35cd1-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="35cd1-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="35cd1-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="35cd1-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cd1-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="35cd1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35cd1-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35cd1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35cd1-118">Not supported.</span></span>|
|<span data-ttu-id="35cd1-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="35cd1-119">Application</span></span>||
| <span data-ttu-id="35cd1-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="35cd1-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="35cd1-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cd1-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="35cd1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35cd1-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="35cd1-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="35cd1-123">Request headers</span></span>
|<span data-ttu-id="35cd1-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35cd1-124">Header</span></span>|<span data-ttu-id="35cd1-125">Значение</span><span class="sxs-lookup"><span data-stu-id="35cd1-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35cd1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="35cd1-126">Authorization</span></span>|<span data-ttu-id="35cd1-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35cd1-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35cd1-128">Accept</span><span class="sxs-lookup"><span data-stu-id="35cd1-128">Accept</span></span>|<span data-ttu-id="35cd1-129">application/json</span><span class="sxs-lookup"><span data-stu-id="35cd1-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35cd1-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35cd1-130">Request body</span></span>
<span data-ttu-id="35cd1-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35cd1-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="35cd1-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="35cd1-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="35cd1-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="35cd1-133">Property</span></span>|<span data-ttu-id="35cd1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="35cd1-134">Type</span></span>|<span data-ttu-id="35cd1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="35cd1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35cd1-136">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="35cd1-136">notificationTitle</span></span>|<span data-ttu-id="35cd1-137">String</span><span class="sxs-lookup"><span data-stu-id="35cd1-137">String</span></span>|<span data-ttu-id="35cd1-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35cd1-138">Not yet documented</span></span>|
|<span data-ttu-id="35cd1-139">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="35cd1-139">notificationBody</span></span>|<span data-ttu-id="35cd1-140">String</span><span class="sxs-lookup"><span data-stu-id="35cd1-140">String</span></span>|<span data-ttu-id="35cd1-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35cd1-141">Not yet documented</span></span>|
|<span data-ttu-id="35cd1-142">граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="35cd1-142">groupsToNotify</span></span>|<span data-ttu-id="35cd1-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="35cd1-143">String collection</span></span>|<span data-ttu-id="35cd1-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="35cd1-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="35cd1-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="35cd1-145">Response</span></span>
<span data-ttu-id="35cd1-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35cd1-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35cd1-147">Пример</span><span class="sxs-lookup"><span data-stu-id="35cd1-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="35cd1-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="35cd1-148">Request</span></span>
<span data-ttu-id="35cd1-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35cd1-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35cd1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="35cd1-150">Response</span></span>
<span data-ttu-id="35cd1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35cd1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












