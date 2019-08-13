---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efdadb8e5e87eecf0d70102d261a9f4d87a6468a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347559"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="06c82-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="06c82-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="06c82-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06c82-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06c82-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06c82-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06c82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c82-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06c82-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06c82-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06c82-108">Prerequisites</span></span>
<span data-ttu-id="06c82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06c82-111">Permission type</span></span>|<span data-ttu-id="06c82-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06c82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06c82-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="06c82-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="06c82-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="06c82-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c82-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06c82-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06c82-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c82-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c82-117">Not supported.</span></span>|
|<span data-ttu-id="06c82-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06c82-118">Application</span></span>|<span data-ttu-id="06c82-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c82-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c82-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06c82-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="06c82-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06c82-121">Request headers</span></span>
|<span data-ttu-id="06c82-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06c82-122">Header</span></span>|<span data-ttu-id="06c82-123">Значение</span><span class="sxs-lookup"><span data-stu-id="06c82-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c82-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06c82-124">Authorization</span></span>|<span data-ttu-id="06c82-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c82-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c82-126">Accept</span><span class="sxs-lookup"><span data-stu-id="06c82-126">Accept</span></span>|<span data-ttu-id="06c82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="06c82-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c82-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06c82-128">Request body</span></span>
<span data-ttu-id="06c82-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06c82-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="06c82-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="06c82-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="06c82-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c82-131">Property</span></span>|<span data-ttu-id="06c82-132">Тип</span><span class="sxs-lookup"><span data-stu-id="06c82-132">Type</span></span>|<span data-ttu-id="06c82-133">Описание</span><span class="sxs-lookup"><span data-stu-id="06c82-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c82-134">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="06c82-134">notificationTitle</span></span>|<span data-ttu-id="06c82-135">String</span><span class="sxs-lookup"><span data-stu-id="06c82-135">String</span></span>|<span data-ttu-id="06c82-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06c82-136">Not yet documented</span></span>|
|<span data-ttu-id="06c82-137">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="06c82-137">notificationBody</span></span>|<span data-ttu-id="06c82-138">String</span><span class="sxs-lookup"><span data-stu-id="06c82-138">String</span></span>|<span data-ttu-id="06c82-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06c82-139">Not yet documented</span></span>|
|<span data-ttu-id="06c82-140">граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="06c82-140">groupsToNotify</span></span>|<span data-ttu-id="06c82-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="06c82-141">String collection</span></span>|<span data-ttu-id="06c82-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06c82-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06c82-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="06c82-143">Response</span></span>
<span data-ttu-id="06c82-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06c82-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06c82-145">Пример</span><span class="sxs-lookup"><span data-stu-id="06c82-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="06c82-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="06c82-146">Request</span></span>
<span data-ttu-id="06c82-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06c82-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06c82-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="06c82-148">Response</span></span>
<span data-ttu-id="06c82-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06c82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









