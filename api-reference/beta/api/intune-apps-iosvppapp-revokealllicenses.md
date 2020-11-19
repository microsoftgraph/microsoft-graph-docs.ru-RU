---
title: Действие revokeAllLicenses
description: Отозвать все назначенные лицензии на Android для данного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6eae639a694d2e23d437453c07c0c0a71f8bb4b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252398"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="cf5c0-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="cf5c0-103">revokeAllLicenses action</span></span>

<span data-ttu-id="cf5c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf5c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf5c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf5c0-107">Отозвать все назначенные лицензии на Android для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-107">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf5c0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf5c0-108">Prerequisites</span></span>
<span data-ttu-id="cf5c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5c0-111">Permission type</span></span>|<span data-ttu-id="cf5c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf5c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf5c0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5c0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf5c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf5c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf5c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-116">Not supported.</span></span>|
|<span data-ttu-id="cf5c0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf5c0-117">Application</span></span>|<span data-ttu-id="cf5c0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5c0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf5c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf5c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="cf5c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf5c0-120">Request headers</span></span>
|<span data-ttu-id="cf5c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf5c0-121">Header</span></span>|<span data-ttu-id="cf5c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf5c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf5c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf5c0-123">Authorization</span></span>|<span data-ttu-id="cf5c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf5c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf5c0-125">Accept</span></span>|<span data-ttu-id="cf5c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf5c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf5c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf5c0-127">Request body</span></span>
<span data-ttu-id="cf5c0-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cf5c0-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cf5c0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf5c0-130">Property</span></span>|<span data-ttu-id="cf5c0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf5c0-131">Type</span></span>|<span data-ttu-id="cf5c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5c0-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="cf5c0-133">notifyManagedDevices</span></span>|<span data-ttu-id="cf5c0-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf5c0-134">Boolean</span></span>|<span data-ttu-id="cf5c0-135">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="cf5c0-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="cf5c0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf5c0-136">Response</span></span>
<span data-ttu-id="cf5c0-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf5c0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cf5c0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf5c0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf5c0-139">Request</span></span>
<span data-ttu-id="cf5c0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="cf5c0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5c0-141">Response</span></span>
<span data-ttu-id="cf5c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf5c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




