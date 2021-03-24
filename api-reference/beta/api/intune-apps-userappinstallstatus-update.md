---
title: Обновление userAppInstallStatus
description: Обновление свойств объекта userAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10bd4b5a9064036e6e3d40fb4ac6334f8aada1d9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142956"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="59949-103">Обновление userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="59949-103">Update userAppInstallStatus</span></span>

<span data-ttu-id="59949-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59949-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59949-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59949-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59949-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59949-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59949-107">Обновление свойств объекта [userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59949-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59949-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59949-108">Prerequisites</span></span>
<span data-ttu-id="59949-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59949-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59949-111">Permission type</span></span>|<span data-ttu-id="59949-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59949-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59949-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59949-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59949-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59949-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59949-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59949-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59949-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59949-116">Not supported.</span></span>|
|<span data-ttu-id="59949-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="59949-117">Application</span></span>|<span data-ttu-id="59949-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59949-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59949-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59949-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="59949-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="59949-120">Request headers</span></span>
|<span data-ttu-id="59949-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59949-121">Header</span></span>|<span data-ttu-id="59949-122">Значение</span><span class="sxs-lookup"><span data-stu-id="59949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59949-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59949-123">Authorization</span></span>|<span data-ttu-id="59949-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59949-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59949-125">Accept</span></span>|<span data-ttu-id="59949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59949-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59949-127">Request body</span></span>
<span data-ttu-id="59949-128">В теле запроса поставляем представление JSON для [объекта userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59949-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="59949-129">В следующей таблице показаны свойства, необходимые при создании [userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59949-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="59949-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="59949-130">Property</span></span>|<span data-ttu-id="59949-131">Тип</span><span class="sxs-lookup"><span data-stu-id="59949-131">Type</span></span>|<span data-ttu-id="59949-132">Описание</span><span class="sxs-lookup"><span data-stu-id="59949-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59949-133">id</span><span class="sxs-lookup"><span data-stu-id="59949-133">id</span></span>|<span data-ttu-id="59949-134">Строка</span><span class="sxs-lookup"><span data-stu-id="59949-134">String</span></span>|<span data-ttu-id="59949-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59949-135">Key of the entity.</span></span>|
|<span data-ttu-id="59949-136">userName</span><span class="sxs-lookup"><span data-stu-id="59949-136">userName</span></span>|<span data-ttu-id="59949-137">String</span><span class="sxs-lookup"><span data-stu-id="59949-137">String</span></span>|<span data-ttu-id="59949-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="59949-138">User name.</span></span>|
|<span data-ttu-id="59949-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="59949-139">userPrincipalName</span></span>|<span data-ttu-id="59949-140">String</span><span class="sxs-lookup"><span data-stu-id="59949-140">String</span></span>|<span data-ttu-id="59949-141">Имя главного пользователя.</span><span class="sxs-lookup"><span data-stu-id="59949-141">User Principal Name.</span></span>|
|<span data-ttu-id="59949-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59949-142">installedDeviceCount</span></span>|<span data-ttu-id="59949-143">Int32</span><span class="sxs-lookup"><span data-stu-id="59949-143">Int32</span></span>|<span data-ttu-id="59949-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="59949-144">Installed Device Count.</span></span>|
|<span data-ttu-id="59949-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59949-145">failedDeviceCount</span></span>|<span data-ttu-id="59949-146">Int32</span><span class="sxs-lookup"><span data-stu-id="59949-146">Int32</span></span>|<span data-ttu-id="59949-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="59949-147">Failed Device Count.</span></span>|
|<span data-ttu-id="59949-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59949-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="59949-149">Int32</span><span class="sxs-lookup"><span data-stu-id="59949-149">Int32</span></span>|<span data-ttu-id="59949-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="59949-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="59949-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="59949-151">Response</span></span>
<span data-ttu-id="59949-152">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59949-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59949-153">Пример</span><span class="sxs-lookup"><span data-stu-id="59949-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="59949-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="59949-154">Request</span></span>
<span data-ttu-id="59949-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59949-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="59949-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="59949-156">Response</span></span>
<span data-ttu-id="59949-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59949-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




