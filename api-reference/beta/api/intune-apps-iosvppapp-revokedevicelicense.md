---
title: Действие revokeAllLicenses
description: Отзыв назначенной лицензии на устройство VPP для iOS для данного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7436c6a98f5a3d2c2c73bc8ce1c5776b0545b94
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761946"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="0a3c9-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="0a3c9-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="0a3c9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a3c9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a3c9-106">Отзыв назначенной лицензии на устройство VPP для iOS для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a3c9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a3c9-107">Prerequisites</span></span>
<span data-ttu-id="0a3c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3c9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3c9-110">Permission type</span></span>|<span data-ttu-id="0a3c9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a3c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3c9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a3c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3c9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3c9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a3c9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a3c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-115">Not supported.</span></span>|
|<span data-ttu-id="0a3c9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a3c9-116">Application</span></span>|<span data-ttu-id="0a3c9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3c9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3c9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a3c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="0a3c9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a3c9-119">Request headers</span></span>
|<span data-ttu-id="0a3c9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a3c9-120">Header</span></span>|<span data-ttu-id="0a3c9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0a3c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a3c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a3c9-122">Authorization</span></span>|<span data-ttu-id="0a3c9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a3c9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0a3c9-124">Accept</span></span>|<span data-ttu-id="0a3c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a3c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3c9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a3c9-126">Request body</span></span>
<span data-ttu-id="0a3c9-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a3c9-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a3c9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a3c9-129">Property</span></span>|<span data-ttu-id="0a3c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0a3c9-130">Type</span></span>|<span data-ttu-id="0a3c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0a3c9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a3c9-132">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="0a3c9-132">managedDeviceId</span></span>|<span data-ttu-id="0a3c9-133">String</span><span class="sxs-lookup"><span data-stu-id="0a3c9-133">String</span></span>|<span data-ttu-id="0a3c9-134">DeviceId, для которого назначена лицензия на приложение</span><span class="sxs-lookup"><span data-stu-id="0a3c9-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="0a3c9-135">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="0a3c9-135">notifyManagedDevices</span></span>|<span data-ttu-id="0a3c9-136">Логический</span><span class="sxs-lookup"><span data-stu-id="0a3c9-136">Boolean</span></span>|<span data-ttu-id="0a3c9-137">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="0a3c9-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="0a3c9-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a3c9-138">Response</span></span>
<span data-ttu-id="0a3c9-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a3c9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0a3c9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a3c9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a3c9-141">Request</span></span>
<span data-ttu-id="0a3c9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="0a3c9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3c9-143">Response</span></span>
<span data-ttu-id="0a3c9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a3c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




