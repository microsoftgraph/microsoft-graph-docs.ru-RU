---
title: Действие revokeAllLicenses
description: Отзывать назначенную лицензию на устройство VPP iOS для данного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 648677f00c26c4432614eda9ce840b152528a5e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144104"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="fbfae-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="fbfae-103">revokeDeviceLicense action</span></span>

<span data-ttu-id="fbfae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbfae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbfae-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbfae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbfae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbfae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbfae-107">Отзывать назначенную лицензию на устройство VPP iOS для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="fbfae-107">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbfae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fbfae-108">Prerequisites</span></span>
<span data-ttu-id="fbfae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbfae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbfae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbfae-111">Permission type</span></span>|<span data-ttu-id="fbfae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbfae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbfae-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbfae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbfae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbfae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbfae-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbfae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbfae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbfae-116">Not supported.</span></span>|
|<span data-ttu-id="fbfae-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fbfae-117">Application</span></span>|<span data-ttu-id="fbfae-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbfae-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbfae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbfae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="fbfae-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbfae-120">Request headers</span></span>
|<span data-ttu-id="fbfae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbfae-121">Header</span></span>|<span data-ttu-id="fbfae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbfae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbfae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbfae-123">Authorization</span></span>|<span data-ttu-id="fbfae-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbfae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbfae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbfae-125">Accept</span></span>|<span data-ttu-id="fbfae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbfae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbfae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbfae-127">Request body</span></span>
<span data-ttu-id="fbfae-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbfae-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fbfae-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fbfae-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fbfae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbfae-130">Property</span></span>|<span data-ttu-id="fbfae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbfae-131">Type</span></span>|<span data-ttu-id="fbfae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbfae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfae-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fbfae-133">managedDeviceId</span></span>|<span data-ttu-id="fbfae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fbfae-134">String</span></span>|<span data-ttu-id="fbfae-135">DeviceId, для которого будет отозвана назначенная лицензия приложения</span><span class="sxs-lookup"><span data-stu-id="fbfae-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="fbfae-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="fbfae-136">notifyManagedDevices</span></span>|<span data-ttu-id="fbfae-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbfae-137">Boolean</span></span>|<span data-ttu-id="fbfae-138">Boolean, который указывает, следует ли отправить уведомление об отводе на устройство</span><span class="sxs-lookup"><span data-stu-id="fbfae-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="fbfae-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbfae-139">Response</span></span>
<span data-ttu-id="fbfae-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fbfae-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fbfae-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fbfae-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbfae-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbfae-142">Request</span></span>
<span data-ttu-id="fbfae-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbfae-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="fbfae-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbfae-144">Response</span></span>
<span data-ttu-id="fbfae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbfae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




