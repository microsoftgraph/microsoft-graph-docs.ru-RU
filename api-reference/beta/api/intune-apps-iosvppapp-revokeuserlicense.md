---
title: Действие revokeAllLicenses
description: Отзыв назначенной лицензии пользователя на iOS VPP для данного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd216543ff651dbfe603e3ac7a981fcde3b1c0e7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761939"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="98d75-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="98d75-103">revokeUserLicense action</span></span>

> <span data-ttu-id="98d75-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98d75-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98d75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98d75-106">Отзыв назначенной лицензии пользователя на iOS VPP для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="98d75-106">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98d75-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98d75-107">Prerequisites</span></span>
<span data-ttu-id="98d75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d75-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98d75-110">Permission type</span></span>|<span data-ttu-id="98d75-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98d75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98d75-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98d75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98d75-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d75-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98d75-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98d75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98d75-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d75-115">Not supported.</span></span>|
|<span data-ttu-id="98d75-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="98d75-116">Application</span></span>|<span data-ttu-id="98d75-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d75-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98d75-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98d75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="98d75-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98d75-119">Request headers</span></span>
|<span data-ttu-id="98d75-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98d75-120">Header</span></span>|<span data-ttu-id="98d75-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98d75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98d75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d75-122">Authorization</span></span>|<span data-ttu-id="98d75-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98d75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98d75-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98d75-124">Accept</span></span>|<span data-ttu-id="98d75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98d75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d75-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98d75-126">Request body</span></span>
<span data-ttu-id="98d75-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98d75-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="98d75-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="98d75-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="98d75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="98d75-129">Property</span></span>|<span data-ttu-id="98d75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="98d75-130">Type</span></span>|<span data-ttu-id="98d75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="98d75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98d75-132">userId</span><span class="sxs-lookup"><span data-stu-id="98d75-132">userId</span></span>|<span data-ttu-id="98d75-133">String</span><span class="sxs-lookup"><span data-stu-id="98d75-133">String</span></span>|<span data-ttu-id="98d75-134">Идентификатор пользователя, которому назначена лицензия на приложение</span><span class="sxs-lookup"><span data-stu-id="98d75-134">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="98d75-135">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="98d75-135">notifyManagedDevices</span></span>|<span data-ttu-id="98d75-136">Логический</span><span class="sxs-lookup"><span data-stu-id="98d75-136">Boolean</span></span>|<span data-ttu-id="98d75-137">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="98d75-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="98d75-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="98d75-138">Response</span></span>
<span data-ttu-id="98d75-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98d75-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98d75-140">Пример</span><span class="sxs-lookup"><span data-stu-id="98d75-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="98d75-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="98d75-141">Request</span></span>
<span data-ttu-id="98d75-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98d75-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="98d75-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="98d75-143">Response</span></span>
<span data-ttu-id="98d75-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98d75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




