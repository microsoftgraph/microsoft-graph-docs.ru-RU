---
title: Действие revokeDeviceLicense
description: Лицензии устройства VPP REVOKE назначенных операций ввода-вывода для заданного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b58fe7440b1b77e5dc651a4a7c802dae8e5139c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410408"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="8011c-103">Действие revokeDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="8011c-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="8011c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8011c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8011c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8011c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8011c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8011c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8011c-107">Лицензии устройства VPP REVOKE назначенных операций ввода-вывода для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="8011c-107">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8011c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8011c-108">Prerequisites</span></span>
<span data-ttu-id="8011c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8011c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8011c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8011c-111">Permission type</span></span>|<span data-ttu-id="8011c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8011c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8011c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8011c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8011c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8011c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8011c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8011c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8011c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8011c-116">Not supported.</span></span>|
|<span data-ttu-id="8011c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8011c-117">Application</span></span>|<span data-ttu-id="8011c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8011c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8011c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8011c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="8011c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8011c-120">Request headers</span></span>
|<span data-ttu-id="8011c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8011c-121">Header</span></span>|<span data-ttu-id="8011c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8011c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8011c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8011c-123">Authorization</span></span>|<span data-ttu-id="8011c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8011c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8011c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8011c-125">Accept</span></span>|<span data-ttu-id="8011c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8011c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8011c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8011c-127">Request body</span></span>
<span data-ttu-id="8011c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8011c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8011c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8011c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8011c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8011c-130">Property</span></span>|<span data-ttu-id="8011c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8011c-131">Type</span></span>|<span data-ttu-id="8011c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8011c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8011c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8011c-133">managedDeviceId</span></span>|<span data-ttu-id="8011c-134">String</span><span class="sxs-lookup"><span data-stu-id="8011c-134">String</span></span>|<span data-ttu-id="8011c-135">DeviceId, для которого является отозвать лицензии назначенные приложения</span><span class="sxs-lookup"><span data-stu-id="8011c-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="8011c-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="8011c-136">notifyManagedDevices</span></span>|<span data-ttu-id="8011c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="8011c-137">Boolean</span></span>|<span data-ttu-id="8011c-138">Логическое значение, указывающее, если устройство отправляется уведомление revoke</span><span class="sxs-lookup"><span data-stu-id="8011c-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="8011c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8011c-139">Response</span></span>
<span data-ttu-id="8011c-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8011c-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8011c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8011c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8011c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8011c-142">Request</span></span>
<span data-ttu-id="8011c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8011c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="8011c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8011c-144">Response</span></span>
<span data-ttu-id="8011c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8011c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




