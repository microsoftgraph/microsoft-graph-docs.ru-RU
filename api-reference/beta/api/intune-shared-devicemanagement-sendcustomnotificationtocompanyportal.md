---
title: Действие sendCustomNotificationToCompanyPortal
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43e0a5a9690d3f60f646eb5ed55e6d51ba2caab8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418668"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="c3337-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c3337-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="c3337-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3337-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3337-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3337-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3337-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3337-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3337-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3337-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3337-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3337-108">Prerequisites</span></span>
<span data-ttu-id="c3337-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3337-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3337-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3337-111">Permission type</span></span>|<span data-ttu-id="c3337-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3337-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3337-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3337-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c3337-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c3337-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c3337-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3337-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c3337-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3337-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3337-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3337-117">Not supported.</span></span>|
|<span data-ttu-id="c3337-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3337-118">Application</span></span>|<span data-ttu-id="c3337-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3337-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3337-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3337-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="c3337-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3337-121">Request headers</span></span>
|<span data-ttu-id="c3337-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3337-122">Header</span></span>|<span data-ttu-id="c3337-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c3337-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3337-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3337-124">Authorization</span></span>|<span data-ttu-id="c3337-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3337-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3337-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c3337-126">Accept</span></span>|<span data-ttu-id="c3337-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3337-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3337-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3337-128">Request body</span></span>
<span data-ttu-id="c3337-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3337-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c3337-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c3337-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c3337-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3337-131">Property</span></span>|<span data-ttu-id="c3337-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c3337-132">Type</span></span>|<span data-ttu-id="c3337-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c3337-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3337-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="c3337-134">notificationTitle</span></span>|<span data-ttu-id="c3337-135">String</span><span class="sxs-lookup"><span data-stu-id="c3337-135">String</span></span>|<span data-ttu-id="c3337-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3337-136">Not yet documented</span></span>|
|<span data-ttu-id="c3337-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="c3337-137">notificationBody</span></span>|<span data-ttu-id="c3337-138">String</span><span class="sxs-lookup"><span data-stu-id="c3337-138">String</span></span>|<span data-ttu-id="c3337-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3337-139">Not yet documented</span></span>|
|<span data-ttu-id="c3337-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="c3337-140">groupsToNotify</span></span>|<span data-ttu-id="c3337-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3337-141">String collection</span></span>|<span data-ttu-id="c3337-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3337-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c3337-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3337-143">Response</span></span>
<span data-ttu-id="c3337-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3337-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3337-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c3337-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3337-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3337-146">Request</span></span>
<span data-ttu-id="c3337-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3337-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3337-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3337-148">Response</span></span>
<span data-ttu-id="c3337-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3337-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






