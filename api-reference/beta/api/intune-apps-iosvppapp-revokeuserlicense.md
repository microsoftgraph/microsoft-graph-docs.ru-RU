---
title: Действие revokeAllLicenses
description: Отзыв назначенной лицензии пользователя на iOS VPP для данного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b156e34eda17f310afd2f65a4d013f5377b0162
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252293"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="e72aa-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="e72aa-103">revokeUserLicense action</span></span>

<span data-ttu-id="e72aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e72aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e72aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e72aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e72aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e72aa-107">Отзыв назначенной лицензии пользователя на iOS VPP для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="e72aa-107">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e72aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e72aa-108">Prerequisites</span></span>
<span data-ttu-id="e72aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e72aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e72aa-111">Permission type</span></span>|<span data-ttu-id="e72aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e72aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e72aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e72aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e72aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e72aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72aa-116">Not supported.</span></span>|
|<span data-ttu-id="e72aa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e72aa-117">Application</span></span>|<span data-ttu-id="e72aa-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72aa-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e72aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="e72aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e72aa-120">Request headers</span></span>
|<span data-ttu-id="e72aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e72aa-121">Header</span></span>|<span data-ttu-id="e72aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e72aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e72aa-123">Authorization</span></span>|<span data-ttu-id="e72aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e72aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e72aa-125">Accept</span></span>|<span data-ttu-id="e72aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e72aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72aa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e72aa-127">Request body</span></span>
<span data-ttu-id="e72aa-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e72aa-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e72aa-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e72aa-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e72aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e72aa-130">Property</span></span>|<span data-ttu-id="e72aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e72aa-131">Type</span></span>|<span data-ttu-id="e72aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e72aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e72aa-133">userId</span><span class="sxs-lookup"><span data-stu-id="e72aa-133">userId</span></span>|<span data-ttu-id="e72aa-134">String</span><span class="sxs-lookup"><span data-stu-id="e72aa-134">String</span></span>|<span data-ttu-id="e72aa-135">Идентификатор пользователя, которому назначена лицензия на приложение</span><span class="sxs-lookup"><span data-stu-id="e72aa-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="e72aa-136">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="e72aa-136">notifyManagedDevices</span></span>|<span data-ttu-id="e72aa-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e72aa-137">Boolean</span></span>|<span data-ttu-id="e72aa-138">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="e72aa-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="e72aa-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e72aa-139">Response</span></span>
<span data-ttu-id="e72aa-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e72aa-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e72aa-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e72aa-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72aa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e72aa-142">Request</span></span>
<span data-ttu-id="e72aa-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e72aa-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="e72aa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e72aa-144">Response</span></span>
<span data-ttu-id="e72aa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e72aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




