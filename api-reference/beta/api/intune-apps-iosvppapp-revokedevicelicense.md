---
title: Действие revokeAllLicenses
description: Отзыв назначенной лицензии на устройство VPP для iOS для данного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0ffc1ec83a4253a6c06a059f420630e25896df2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173572"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="a5fc3-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="a5fc3-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="a5fc3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5fc3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5fc3-106">Отзыв назначенной лицензии на устройство VPP для iOS для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5fc3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a5fc3-107">Prerequisites</span></span>
<span data-ttu-id="a5fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5fc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fc3-110">Permission type</span></span>|<span data-ttu-id="a5fc3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5fc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5fc3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fc3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5fc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5fc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-115">Not supported.</span></span>|
|<span data-ttu-id="a5fc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5fc3-116">Application</span></span>|<span data-ttu-id="a5fc3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fc3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5fc3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="a5fc3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5fc3-119">Request headers</span></span>
|<span data-ttu-id="a5fc3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5fc3-120">Header</span></span>|<span data-ttu-id="a5fc3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5fc3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5fc3-122">Authorization</span></span>|<span data-ttu-id="a5fc3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5fc3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5fc3-124">Accept</span></span>|<span data-ttu-id="a5fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5fc3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5fc3-126">Request body</span></span>
<span data-ttu-id="a5fc3-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5fc3-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5fc3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5fc3-129">Property</span></span>|<span data-ttu-id="a5fc3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5fc3-130">Type</span></span>|<span data-ttu-id="a5fc3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fc3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5fc3-132">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="a5fc3-132">managedDeviceId</span></span>|<span data-ttu-id="a5fc3-133">String.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-133">String</span></span>|<span data-ttu-id="a5fc3-134">DeviceId, для которого назначена лицензия на приложение</span><span class="sxs-lookup"><span data-stu-id="a5fc3-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="a5fc3-135">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="a5fc3-135">notifyManagedDevices</span></span>|<span data-ttu-id="a5fc3-136">Boolean.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-136">Boolean</span></span>|<span data-ttu-id="a5fc3-137">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="a5fc3-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="a5fc3-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5fc3-138">Response</span></span>
<span data-ttu-id="a5fc3-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5fc3-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a5fc3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5fc3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5fc3-141">Request</span></span>
<span data-ttu-id="a5fc3-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="a5fc3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fc3-143">Response</span></span>
<span data-ttu-id="a5fc3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5fc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




