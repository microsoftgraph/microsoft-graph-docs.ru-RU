---
title: Действие revokeDeviceLicense
description: Лицензии устройства VPP REVOKE назначенных операций ввода-вывода для заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a8dca4ea62e08e9d34727dd2142a156ba2d8dee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864976"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="d9474-103">Действие revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="d9474-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="d9474-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9474-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9474-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9474-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9474-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d9474-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9474-107">Лицензии устройства VPP REVOKE назначенных операций ввода-вывода для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="d9474-107">Revoke assigned iOS VPP device license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9474-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9474-108">Prerequisites</span></span>
<span data-ttu-id="d9474-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9474-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9474-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9474-111">Permission type</span></span>|<span data-ttu-id="d9474-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9474-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9474-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9474-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9474-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9474-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9474-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9474-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9474-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9474-116">Not supported.</span></span>|
|<span data-ttu-id="d9474-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9474-117">Application</span></span>|<span data-ttu-id="d9474-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9474-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9474-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9474-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="d9474-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9474-120">Request headers</span></span>
|<span data-ttu-id="d9474-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9474-121">Header</span></span>|<span data-ttu-id="d9474-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9474-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9474-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9474-123">Authorization</span></span>|<span data-ttu-id="d9474-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d9474-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9474-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9474-125">Accept</span></span>|<span data-ttu-id="d9474-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9474-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9474-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9474-127">Request body</span></span>
<span data-ttu-id="d9474-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9474-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9474-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d9474-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9474-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9474-130">Property</span></span>|<span data-ttu-id="d9474-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9474-131">Type</span></span>|<span data-ttu-id="d9474-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9474-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9474-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d9474-133">managedDeviceId</span></span>|<span data-ttu-id="d9474-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d9474-134">String</span></span>|<span data-ttu-id="d9474-135">DeviceId, для которого является отозвать лицензии назначенные приложения</span><span class="sxs-lookup"><span data-stu-id="d9474-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="d9474-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="d9474-136">notifyManagedDevices</span></span>|<span data-ttu-id="d9474-137">Логический</span><span class="sxs-lookup"><span data-stu-id="d9474-137">Boolean</span></span>|<span data-ttu-id="d9474-138">Логическое значение, указывающее, если устройство отправляется уведомление revoke</span><span class="sxs-lookup"><span data-stu-id="d9474-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="d9474-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9474-139">Response</span></span>
<span data-ttu-id="d9474-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9474-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9474-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d9474-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9474-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9474-142">Request</span></span>
<span data-ttu-id="d9474-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9474-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="d9474-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9474-144">Response</span></span>
<span data-ttu-id="d9474-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d9474-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





