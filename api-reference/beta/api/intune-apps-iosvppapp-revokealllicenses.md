---
title: Действие revokeAllLicenses
description: Отозвать все назначенные лицензии на Android для данного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9850ff5ed3a3c9f382d0d2faa3a9cdcb97e3986
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169813"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="891d4-103">Действие revokeAllLicenses</span><span class="sxs-lookup"><span data-stu-id="891d4-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="891d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891d4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="891d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891d4-106">Отозвать все назначенные лицензии на Android для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="891d4-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="891d4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="891d4-107">Prerequisites</span></span>
<span data-ttu-id="891d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="891d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="891d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="891d4-110">Permission type</span></span>|<span data-ttu-id="891d4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="891d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="891d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="891d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="891d4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891d4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="891d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="891d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="891d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891d4-115">Not supported.</span></span>|
|<span data-ttu-id="891d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="891d4-116">Application</span></span>|<span data-ttu-id="891d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="891d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="891d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="891d4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="891d4-119">Request headers</span></span>
|<span data-ttu-id="891d4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="891d4-120">Header</span></span>|<span data-ttu-id="891d4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="891d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="891d4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="891d4-122">Authorization</span></span>|<span data-ttu-id="891d4-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="891d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="891d4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="891d4-124">Accept</span></span>|<span data-ttu-id="891d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="891d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="891d4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="891d4-126">Request body</span></span>
<span data-ttu-id="891d4-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="891d4-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="891d4-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="891d4-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="891d4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="891d4-129">Property</span></span>|<span data-ttu-id="891d4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="891d4-130">Type</span></span>|<span data-ttu-id="891d4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="891d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891d4-132">Нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="891d4-132">notifyManagedDevices</span></span>|<span data-ttu-id="891d4-133">Логический</span><span class="sxs-lookup"><span data-stu-id="891d4-133">Boolean</span></span>|<span data-ttu-id="891d4-134">Логическое значение, указывающее, следует ли отправлять уведомление об отзыве на устройство</span><span class="sxs-lookup"><span data-stu-id="891d4-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="891d4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="891d4-135">Response</span></span>
<span data-ttu-id="891d4-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="891d4-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="891d4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="891d4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="891d4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="891d4-138">Request</span></span>
<span data-ttu-id="891d4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="891d4-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="891d4-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="891d4-140">Response</span></span>
<span data-ttu-id="891d4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="891d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




