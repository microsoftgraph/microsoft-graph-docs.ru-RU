---
title: Создание Усераппинсталлстатус
description: Создание нового объекта Усераппинсталлстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8fae76fcc240a3aada2fcc5d8f7eec610ddd368
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444877"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="599d9-103">Создание Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="599d9-103">Create userAppInstallStatus</span></span>

<span data-ttu-id="599d9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="599d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="599d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="599d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="599d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="599d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="599d9-107">Создание нового объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="599d9-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="599d9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="599d9-108">Prerequisites</span></span>
<span data-ttu-id="599d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="599d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="599d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="599d9-111">Permission type</span></span>|<span data-ttu-id="599d9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="599d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="599d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="599d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="599d9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599d9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="599d9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="599d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="599d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="599d9-116">Not supported.</span></span>|
|<span data-ttu-id="599d9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="599d9-117">Application</span></span>|<span data-ttu-id="599d9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599d9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="599d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="599d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="599d9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="599d9-120">Request headers</span></span>
|<span data-ttu-id="599d9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="599d9-121">Header</span></span>|<span data-ttu-id="599d9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="599d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="599d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="599d9-123">Authorization</span></span>|<span data-ttu-id="599d9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="599d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="599d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="599d9-125">Accept</span></span>|<span data-ttu-id="599d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="599d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="599d9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="599d9-127">Request body</span></span>
<span data-ttu-id="599d9-128">В тексте запроса добавьте представление объекта Усераппинсталлстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="599d9-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="599d9-129">В следующей таблице приведены свойства, необходимые при создании Усераппинсталлстатус.</span><span class="sxs-lookup"><span data-stu-id="599d9-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="599d9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="599d9-130">Property</span></span>|<span data-ttu-id="599d9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="599d9-131">Type</span></span>|<span data-ttu-id="599d9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="599d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="599d9-133">id</span><span class="sxs-lookup"><span data-stu-id="599d9-133">id</span></span>|<span data-ttu-id="599d9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="599d9-134">String</span></span>|<span data-ttu-id="599d9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="599d9-135">Key of the entity.</span></span>|
|<span data-ttu-id="599d9-136">userName</span><span class="sxs-lookup"><span data-stu-id="599d9-136">userName</span></span>|<span data-ttu-id="599d9-137">String</span><span class="sxs-lookup"><span data-stu-id="599d9-137">String</span></span>|<span data-ttu-id="599d9-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="599d9-138">User name.</span></span>|
|<span data-ttu-id="599d9-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="599d9-139">userPrincipalName</span></span>|<span data-ttu-id="599d9-140">String</span><span class="sxs-lookup"><span data-stu-id="599d9-140">String</span></span>|<span data-ttu-id="599d9-141">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="599d9-141">User Principal Name.</span></span>|
|<span data-ttu-id="599d9-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="599d9-142">installedDeviceCount</span></span>|<span data-ttu-id="599d9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="599d9-143">Int32</span></span>|<span data-ttu-id="599d9-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="599d9-144">Installed Device Count.</span></span>|
|<span data-ttu-id="599d9-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="599d9-145">failedDeviceCount</span></span>|<span data-ttu-id="599d9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="599d9-146">Int32</span></span>|<span data-ttu-id="599d9-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="599d9-147">Failed Device Count.</span></span>|
|<span data-ttu-id="599d9-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="599d9-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="599d9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="599d9-149">Int32</span></span>|<span data-ttu-id="599d9-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="599d9-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="599d9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="599d9-151">Response</span></span>
<span data-ttu-id="599d9-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="599d9-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="599d9-153">Пример</span><span class="sxs-lookup"><span data-stu-id="599d9-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="599d9-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="599d9-154">Request</span></span>
<span data-ttu-id="599d9-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="599d9-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="599d9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="599d9-156">Response</span></span>
<span data-ttu-id="599d9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="599d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





