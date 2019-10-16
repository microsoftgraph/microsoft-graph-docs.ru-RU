---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ca315bb06aadd054787d7a5e29d6b9161256a2a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536156"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="b008f-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b008f-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="b008f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b008f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b008f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b008f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b008f-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b008f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b008f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b008f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b008f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b008f-108">Prerequisites</span></span>
<span data-ttu-id="b008f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b008f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b008f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b008f-111">Permission type</span></span>|<span data-ttu-id="b008f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b008f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b008f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b008f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b008f-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b008f-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b008f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b008f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b008f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b008f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b008f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b008f-117">Not supported.</span></span>|
|<span data-ttu-id="b008f-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b008f-118">Application</span></span>||
| <span data-ttu-id="b008f-119">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="b008f-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b008f-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b008f-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="b008f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b008f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="b008f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b008f-122">Request headers</span></span>
|<span data-ttu-id="b008f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b008f-123">Header</span></span>|<span data-ttu-id="b008f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b008f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b008f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b008f-125">Authorization</span></span>|<span data-ttu-id="b008f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b008f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b008f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b008f-127">Accept</span></span>|<span data-ttu-id="b008f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b008f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b008f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b008f-129">Request body</span></span>
<span data-ttu-id="b008f-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b008f-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b008f-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b008f-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b008f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b008f-132">Property</span></span>|<span data-ttu-id="b008f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b008f-133">Type</span></span>|<span data-ttu-id="b008f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b008f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b008f-135">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="b008f-135">notificationTitle</span></span>|<span data-ttu-id="b008f-136">String</span><span class="sxs-lookup"><span data-stu-id="b008f-136">String</span></span>|<span data-ttu-id="b008f-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b008f-137">Not yet documented</span></span>|
|<span data-ttu-id="b008f-138">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="b008f-138">notificationBody</span></span>|<span data-ttu-id="b008f-139">String</span><span class="sxs-lookup"><span data-stu-id="b008f-139">String</span></span>|<span data-ttu-id="b008f-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b008f-140">Not yet documented</span></span>|
|<span data-ttu-id="b008f-141">граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="b008f-141">groupsToNotify</span></span>|<span data-ttu-id="b008f-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b008f-142">String collection</span></span>|<span data-ttu-id="b008f-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b008f-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b008f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b008f-144">Response</span></span>
<span data-ttu-id="b008f-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b008f-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b008f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="b008f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="b008f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="b008f-147">Request</span></span>
<span data-ttu-id="b008f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b008f-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b008f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b008f-149">Response</span></span>
<span data-ttu-id="b008f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b008f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












