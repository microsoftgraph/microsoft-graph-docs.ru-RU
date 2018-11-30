---
title: Действие revokeAllLicenses
description: Операций ввода-вывода REVOKE назначенных VPP лицензируемые для заданного приложения.
ms.openlocfilehash: 576cbf5b63f9eb1f00a409483a36a483bf0c9892
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082053"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="97539-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="97539-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="97539-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97539-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97539-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97539-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97539-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97539-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97539-107">Операций ввода-вывода REVOKE назначенных VPP лицензируемые для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="97539-107">Revoke all assigned iOS VPP licenses for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97539-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97539-108">Prerequisites</span></span>
<span data-ttu-id="97539-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97539-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97539-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97539-111">Permission type</span></span>|<span data-ttu-id="97539-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97539-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97539-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97539-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97539-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97539-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97539-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97539-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97539-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97539-116">Not supported.</span></span>|
|<span data-ttu-id="97539-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97539-117">Application</span></span>|<span data-ttu-id="97539-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97539-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97539-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97539-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="97539-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97539-120">Request headers</span></span>
|<span data-ttu-id="97539-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97539-121">Header</span></span>|<span data-ttu-id="97539-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97539-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97539-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97539-123">Authorization</span></span>|<span data-ttu-id="97539-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="97539-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97539-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97539-125">Accept</span></span>|<span data-ttu-id="97539-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97539-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97539-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97539-127">Request body</span></span>
<span data-ttu-id="97539-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97539-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="97539-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="97539-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="97539-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="97539-130">Property</span></span>|<span data-ttu-id="97539-131">Тип</span><span class="sxs-lookup"><span data-stu-id="97539-131">Type</span></span>|<span data-ttu-id="97539-132">Description</span><span class="sxs-lookup"><span data-stu-id="97539-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97539-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="97539-133">notifyManagedDevices</span></span>|<span data-ttu-id="97539-134">Логический</span><span class="sxs-lookup"><span data-stu-id="97539-134">Boolean</span></span>|<span data-ttu-id="97539-135">Логическое значение, указывающее, если устройство отправляется уведомление revoke</span><span class="sxs-lookup"><span data-stu-id="97539-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="97539-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="97539-136">Response</span></span>
<span data-ttu-id="97539-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97539-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97539-138">Пример</span><span class="sxs-lookup"><span data-stu-id="97539-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="97539-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="97539-139">Request</span></span>
<span data-ttu-id="97539-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97539-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="97539-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="97539-141">Response</span></span>
<span data-ttu-id="97539-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="97539-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





