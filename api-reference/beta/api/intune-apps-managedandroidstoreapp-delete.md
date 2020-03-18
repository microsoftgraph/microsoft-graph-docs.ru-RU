---
title: Delete managedAndroidStoreApp
description: Удаляет объект managedAndroidStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 613cf192c7e0b30f9f231cafd14c101663254fd1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815672"
---
# <a name="delete-managedandroidstoreapp"></a><span data-ttu-id="32bba-103">Delete managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="32bba-103">Delete managedAndroidStoreApp</span></span>

> <span data-ttu-id="32bba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32bba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32bba-106">Удаляет объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="32bba-106">Deletes a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32bba-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="32bba-107">Prerequisites</span></span>
<span data-ttu-id="32bba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32bba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32bba-110">Permission type</span></span>|<span data-ttu-id="32bba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32bba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32bba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32bba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32bba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32bba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32bba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32bba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32bba-115">Not supported.</span></span>|
|<span data-ttu-id="32bba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="32bba-116">Application</span></span>|<span data-ttu-id="32bba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32bba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32bba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="32bba-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32bba-119">Request headers</span></span>
|<span data-ttu-id="32bba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32bba-120">Header</span></span>|<span data-ttu-id="32bba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32bba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32bba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32bba-122">Authorization</span></span>|<span data-ttu-id="32bba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32bba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32bba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32bba-124">Accept</span></span>|<span data-ttu-id="32bba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32bba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32bba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32bba-126">Request body</span></span>
<span data-ttu-id="32bba-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32bba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32bba-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bba-128">Response</span></span>
<span data-ttu-id="32bba-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32bba-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32bba-130">Пример</span><span class="sxs-lookup"><span data-stu-id="32bba-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32bba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="32bba-131">Request</span></span>
<span data-ttu-id="32bba-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32bba-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="32bba-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bba-133">Response</span></span>
<span data-ttu-id="32bba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32bba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




