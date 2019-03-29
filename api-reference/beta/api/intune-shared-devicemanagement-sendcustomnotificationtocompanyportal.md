---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43e0a5a9690d3f60f646eb5ed55e6d51ba2caab8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977053"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="cccd1-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cccd1-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="cccd1-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cccd1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cccd1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cccd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cccd1-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cccd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cccd1-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cccd1-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cccd1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cccd1-108">Prerequisites</span></span>
<span data-ttu-id="cccd1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cccd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cccd1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cccd1-111">Permission type</span></span>|<span data-ttu-id="cccd1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cccd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cccd1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cccd1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cccd1-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="cccd1-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="cccd1-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cccd1-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cccd1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cccd1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cccd1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cccd1-117">Not supported.</span></span>|
|<span data-ttu-id="cccd1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cccd1-118">Application</span></span>|<span data-ttu-id="cccd1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cccd1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cccd1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cccd1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="cccd1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cccd1-121">Request headers</span></span>
|<span data-ttu-id="cccd1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cccd1-122">Header</span></span>|<span data-ttu-id="cccd1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cccd1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cccd1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cccd1-124">Authorization</span></span>|<span data-ttu-id="cccd1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cccd1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cccd1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cccd1-126">Accept</span></span>|<span data-ttu-id="cccd1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cccd1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cccd1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cccd1-128">Request body</span></span>
<span data-ttu-id="cccd1-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cccd1-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cccd1-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cccd1-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cccd1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="cccd1-131">Property</span></span>|<span data-ttu-id="cccd1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cccd1-132">Type</span></span>|<span data-ttu-id="cccd1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cccd1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cccd1-134">Нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="cccd1-134">notificationTitle</span></span>|<span data-ttu-id="cccd1-135">String</span><span class="sxs-lookup"><span data-stu-id="cccd1-135">String</span></span>|<span data-ttu-id="cccd1-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cccd1-136">Not yet documented</span></span>|
|<span data-ttu-id="cccd1-137">Нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="cccd1-137">notificationBody</span></span>|<span data-ttu-id="cccd1-138">String</span><span class="sxs-lookup"><span data-stu-id="cccd1-138">String</span></span>|<span data-ttu-id="cccd1-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cccd1-139">Not yet documented</span></span>|
|<span data-ttu-id="cccd1-140">Граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="cccd1-140">groupsToNotify</span></span>|<span data-ttu-id="cccd1-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cccd1-141">String collection</span></span>|<span data-ttu-id="cccd1-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cccd1-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cccd1-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="cccd1-143">Response</span></span>
<span data-ttu-id="cccd1-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cccd1-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cccd1-145">Пример</span><span class="sxs-lookup"><span data-stu-id="cccd1-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="cccd1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="cccd1-146">Request</span></span>
<span data-ttu-id="cccd1-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cccd1-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cccd1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="cccd1-148">Response</span></span>
<span data-ttu-id="cccd1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cccd1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






