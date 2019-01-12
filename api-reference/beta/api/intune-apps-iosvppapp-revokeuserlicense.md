---
title: Действие revokeUserLicense
description: Назначенные REVOKE iOS VPP пользовательской лицензии для заданного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a9c4e61a66bc2a2705586af870708242f21416d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958469"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="4f625-103">Действие revokeUserLicense</span><span class="sxs-lookup"><span data-stu-id="4f625-103">revokeUserLicense action</span></span>

> <span data-ttu-id="4f625-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f625-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f625-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f625-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f625-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f625-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f625-107">Назначенные REVOKE iOS VPP пользовательской лицензии для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="4f625-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f625-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f625-108">Prerequisites</span></span>
<span data-ttu-id="4f625-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f625-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f625-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f625-111">Permission type</span></span>|<span data-ttu-id="4f625-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f625-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f625-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f625-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f625-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f625-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f625-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f625-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f625-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f625-116">Not supported.</span></span>|
|<span data-ttu-id="4f625-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f625-117">Application</span></span>|<span data-ttu-id="4f625-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f625-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f625-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f625-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="4f625-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f625-120">Request headers</span></span>
|<span data-ttu-id="4f625-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f625-121">Header</span></span>|<span data-ttu-id="4f625-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f625-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f625-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f625-123">Authorization</span></span>|<span data-ttu-id="4f625-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4f625-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f625-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f625-125">Accept</span></span>|<span data-ttu-id="4f625-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f625-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f625-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f625-127">Request body</span></span>
<span data-ttu-id="4f625-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f625-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4f625-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4f625-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4f625-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f625-130">Property</span></span>|<span data-ttu-id="4f625-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4f625-131">Type</span></span>|<span data-ttu-id="4f625-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4f625-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f625-133">userId</span><span class="sxs-lookup"><span data-stu-id="4f625-133">userId</span></span>|<span data-ttu-id="4f625-134">String</span><span class="sxs-lookup"><span data-stu-id="4f625-134">String</span></span>|<span data-ttu-id="4f625-135">Идентификатор пользователя, для которого является отозвать лицензии назначенные приложения</span><span class="sxs-lookup"><span data-stu-id="4f625-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="4f625-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="4f625-136">notifyManagedDevices</span></span>|<span data-ttu-id="4f625-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f625-137">Boolean</span></span>|<span data-ttu-id="4f625-138">Логическое значение, указывающее, если устройство отправляется уведомление revoke</span><span class="sxs-lookup"><span data-stu-id="4f625-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="4f625-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f625-139">Response</span></span>
<span data-ttu-id="4f625-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f625-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f625-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4f625-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f625-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f625-142">Request</span></span>
<span data-ttu-id="4f625-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f625-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="4f625-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f625-144">Response</span></span>
<span data-ttu-id="4f625-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f625-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





