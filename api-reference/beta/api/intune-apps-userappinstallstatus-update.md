---
title: Обновление Усераппинсталлстатус
description: Обновление свойств объекта Усераппинсталлстатус.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4a2f4a0c5d9ac75e8abf575913a21a18af571fd9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694874"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="26984-103">Обновление Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="26984-103">Update userAppInstallStatus</span></span>

<span data-ttu-id="26984-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26984-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26984-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26984-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26984-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26984-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26984-107">Обновление свойств объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="26984-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26984-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26984-108">Prerequisites</span></span>
<span data-ttu-id="26984-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26984-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26984-111">Permission type</span></span>|<span data-ttu-id="26984-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26984-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26984-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26984-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26984-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26984-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26984-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26984-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26984-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26984-116">Not supported.</span></span>|
|<span data-ttu-id="26984-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26984-117">Application</span></span>|<span data-ttu-id="26984-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26984-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26984-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26984-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="26984-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26984-120">Request headers</span></span>
|<span data-ttu-id="26984-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26984-121">Header</span></span>|<span data-ttu-id="26984-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26984-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26984-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26984-123">Authorization</span></span>|<span data-ttu-id="26984-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26984-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26984-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26984-125">Accept</span></span>|<span data-ttu-id="26984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26984-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26984-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26984-127">Request body</span></span>
<span data-ttu-id="26984-128">В тексте запроса добавьте представление объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26984-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="26984-129">В следующей таблице приведены свойства, необходимые при создании [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="26984-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="26984-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26984-130">Property</span></span>|<span data-ttu-id="26984-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26984-131">Type</span></span>|<span data-ttu-id="26984-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26984-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26984-133">id</span><span class="sxs-lookup"><span data-stu-id="26984-133">id</span></span>|<span data-ttu-id="26984-134">Строка</span><span class="sxs-lookup"><span data-stu-id="26984-134">String</span></span>|<span data-ttu-id="26984-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26984-135">Key of the entity.</span></span>|
|<span data-ttu-id="26984-136">userName</span><span class="sxs-lookup"><span data-stu-id="26984-136">userName</span></span>|<span data-ttu-id="26984-137">String</span><span class="sxs-lookup"><span data-stu-id="26984-137">String</span></span>|<span data-ttu-id="26984-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="26984-138">User name.</span></span>|
|<span data-ttu-id="26984-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26984-139">userPrincipalName</span></span>|<span data-ttu-id="26984-140">String</span><span class="sxs-lookup"><span data-stu-id="26984-140">String</span></span>|<span data-ttu-id="26984-141">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="26984-141">User Principal Name.</span></span>|
|<span data-ttu-id="26984-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26984-142">installedDeviceCount</span></span>|<span data-ttu-id="26984-143">Int32</span><span class="sxs-lookup"><span data-stu-id="26984-143">Int32</span></span>|<span data-ttu-id="26984-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="26984-144">Installed Device Count.</span></span>|
|<span data-ttu-id="26984-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26984-145">failedDeviceCount</span></span>|<span data-ttu-id="26984-146">Int32</span><span class="sxs-lookup"><span data-stu-id="26984-146">Int32</span></span>|<span data-ttu-id="26984-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="26984-147">Failed Device Count.</span></span>|
|<span data-ttu-id="26984-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26984-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="26984-149">Int32</span><span class="sxs-lookup"><span data-stu-id="26984-149">Int32</span></span>|<span data-ttu-id="26984-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="26984-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="26984-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="26984-151">Response</span></span>
<span data-ttu-id="26984-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26984-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26984-153">Пример</span><span class="sxs-lookup"><span data-stu-id="26984-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="26984-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="26984-154">Request</span></span>
<span data-ttu-id="26984-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26984-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26984-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="26984-156">Response</span></span>
<span data-ttu-id="26984-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26984-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





