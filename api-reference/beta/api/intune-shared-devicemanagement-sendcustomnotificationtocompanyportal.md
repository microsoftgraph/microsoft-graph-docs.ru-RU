---
title: Действие sendCustomNotificationToCompanyPortal
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43e0a5a9690d3f60f646eb5ed55e6d51ba2caab8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527058"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="2cd2d-103">Действие sendCustomNotificationToCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2cd2d-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="2cd2d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cd2d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cd2d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd2d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cd2d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2cd2d-108">Prerequisites</span></span>
<span data-ttu-id="2cd2d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cd2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cd2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cd2d-111">Permission type</span></span>|<span data-ttu-id="2cd2d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cd2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cd2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cd2d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2cd2d-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2cd2d-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2cd2d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cd2d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2cd2d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cd2d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cd2d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-117">Not supported.</span></span>|
|<span data-ttu-id="2cd2d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cd2d-118">Application</span></span>|<span data-ttu-id="2cd2d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cd2d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cd2d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="2cd2d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cd2d-121">Request headers</span></span>
|<span data-ttu-id="2cd2d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cd2d-122">Header</span></span>|<span data-ttu-id="2cd2d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2cd2d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cd2d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cd2d-124">Authorization</span></span>|<span data-ttu-id="2cd2d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cd2d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2cd2d-126">Accept</span></span>|<span data-ttu-id="2cd2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2cd2d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cd2d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cd2d-128">Request body</span></span>
<span data-ttu-id="2cd2d-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2cd2d-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2cd2d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cd2d-131">Property</span></span>|<span data-ttu-id="2cd2d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2cd2d-132">Type</span></span>|<span data-ttu-id="2cd2d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2cd2d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd2d-134">Нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="2cd2d-134">notificationTitle</span></span>|<span data-ttu-id="2cd2d-135">String</span><span class="sxs-lookup"><span data-stu-id="2cd2d-135">String</span></span>|<span data-ttu-id="2cd2d-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-136">Not yet documented</span></span>|
|<span data-ttu-id="2cd2d-137">Нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="2cd2d-137">notificationBody</span></span>|<span data-ttu-id="2cd2d-138">String</span><span class="sxs-lookup"><span data-stu-id="2cd2d-138">String</span></span>|<span data-ttu-id="2cd2d-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-139">Not yet documented</span></span>|
|<span data-ttu-id="2cd2d-140">Граупстонотифи</span><span class="sxs-lookup"><span data-stu-id="2cd2d-140">groupsToNotify</span></span>|<span data-ttu-id="2cd2d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2cd2d-141">String collection</span></span>|<span data-ttu-id="2cd2d-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2cd2d-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2cd2d-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cd2d-143">Response</span></span>
<span data-ttu-id="2cd2d-144">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cd2d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="2cd2d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cd2d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cd2d-146">Request</span></span>
<span data-ttu-id="2cd2d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2cd2d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cd2d-148">Response</span></span>
<span data-ttu-id="2cd2d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cd2d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






