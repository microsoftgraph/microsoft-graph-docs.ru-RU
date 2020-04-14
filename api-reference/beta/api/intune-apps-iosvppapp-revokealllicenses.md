---
title: Действие revokeAllLicenses
description: Отозвать все назначенные лицензии на Android для данного приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1190b70319703e9c1c6ef235131eb86774b1eae6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394550"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="f3081-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="f3081-103">revokeAllLicenses action</span></span>

<span data-ttu-id="f3081-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3081-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3081-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3081-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3081-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3081-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3081-107">Отозвать все назначенные лицензии на Android для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="f3081-107">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3081-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3081-108">Prerequisites</span></span>
<span data-ttu-id="f3081-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3081-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3081-111">Permission type</span></span>|<span data-ttu-id="f3081-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3081-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3081-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3081-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3081-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3081-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3081-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3081-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3081-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3081-116">Not supported.</span></span>|
|<span data-ttu-id="f3081-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f3081-117">Application</span></span>|<span data-ttu-id="f3081-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3081-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3081-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3081-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="f3081-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3081-120">Request headers</span></span>
|<span data-ttu-id="f3081-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3081-121">Header</span></span>|<span data-ttu-id="f3081-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3081-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3081-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3081-123">Authorization</span></span>|<span data-ttu-id="f3081-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3081-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3081-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3081-125">Accept</span></span>|<span data-ttu-id="f3081-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3081-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3081-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3081-127">Request body</span></span>
<span data-ttu-id="f3081-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3081-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f3081-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f3081-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f3081-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3081-130">Property</span></span>|<span data-ttu-id="f3081-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3081-131">Type</span></span>|<span data-ttu-id="f3081-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3081-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3081-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="f3081-133">notifyManagedDevices</span></span>|<span data-ttu-id="f3081-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="f3081-134">Boolean</span></span>|<span data-ttu-id="f3081-135">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="f3081-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="f3081-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3081-136">Response</span></span>
<span data-ttu-id="f3081-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3081-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3081-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f3081-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3081-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3081-139">Request</span></span>
<span data-ttu-id="f3081-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3081-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="f3081-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3081-141">Response</span></span>
<span data-ttu-id="f3081-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3081-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



