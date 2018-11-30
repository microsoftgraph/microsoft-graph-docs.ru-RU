---
title: Действие revokeUserLicense
description: Назначенные REVOKE iOS VPP пользовательской лицензии для заданного приложения.
ms.openlocfilehash: 0222623ba5e1f3de0122a632a3ea9554bbd2c0ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075618"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="d9869-103">Действие revokeUserLicense</span><span class="sxs-lookup"><span data-stu-id="d9869-103">revokeUserLicense action</span></span>

> <span data-ttu-id="d9869-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9869-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9869-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9869-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9869-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d9869-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9869-107">Назначенные REVOKE iOS VPP пользовательской лицензии для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="d9869-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9869-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9869-108">Prerequisites</span></span>
<span data-ttu-id="d9869-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9869-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9869-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9869-111">Permission type</span></span>|<span data-ttu-id="d9869-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9869-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9869-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9869-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9869-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9869-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9869-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9869-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9869-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9869-116">Not supported.</span></span>|
|<span data-ttu-id="d9869-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9869-117">Application</span></span>|<span data-ttu-id="d9869-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9869-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9869-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9869-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="d9869-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9869-120">Request headers</span></span>
|<span data-ttu-id="d9869-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9869-121">Header</span></span>|<span data-ttu-id="d9869-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9869-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9869-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9869-123">Authorization</span></span>|<span data-ttu-id="d9869-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d9869-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9869-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9869-125">Accept</span></span>|<span data-ttu-id="d9869-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9869-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9869-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9869-127">Request body</span></span>
<span data-ttu-id="d9869-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9869-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9869-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d9869-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9869-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9869-130">Property</span></span>|<span data-ttu-id="d9869-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9869-131">Type</span></span>|<span data-ttu-id="d9869-132">Description</span><span class="sxs-lookup"><span data-stu-id="d9869-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9869-133">userId</span><span class="sxs-lookup"><span data-stu-id="d9869-133">userId</span></span>|<span data-ttu-id="d9869-134">String</span><span class="sxs-lookup"><span data-stu-id="d9869-134">String</span></span>|<span data-ttu-id="d9869-135">Идентификатор пользователя, для которого является отозвать лицензии назначенные приложения</span><span class="sxs-lookup"><span data-stu-id="d9869-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="d9869-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="d9869-136">notifyManagedDevices</span></span>|<span data-ttu-id="d9869-137">Логический</span><span class="sxs-lookup"><span data-stu-id="d9869-137">Boolean</span></span>|<span data-ttu-id="d9869-138">Логическое значение, указывающее, если устройство отправляется уведомление revoke</span><span class="sxs-lookup"><span data-stu-id="d9869-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="d9869-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9869-139">Response</span></span>
<span data-ttu-id="d9869-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9869-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9869-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d9869-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9869-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9869-142">Request</span></span>
<span data-ttu-id="d9869-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9869-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="d9869-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9869-144">Response</span></span>
<span data-ttu-id="d9869-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d9869-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





