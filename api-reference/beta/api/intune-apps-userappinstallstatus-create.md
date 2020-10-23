---
title: Создание Усераппинсталлстатус
description: Создание нового объекта Усераппинсталлстатус.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 106d731bfbf4a35b3f7ca3ffeba107e28b1982c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695889"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="b9c8f-103">Создание Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="b9c8f-103">Create userAppInstallStatus</span></span>

<span data-ttu-id="b9c8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9c8f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9c8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c8f-107">Создание нового объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b9c8f-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c8f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9c8f-108">Prerequisites</span></span>
<span data-ttu-id="b9c8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c8f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c8f-111">Permission type</span></span>|<span data-ttu-id="b9c8f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9c8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c8f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9c8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9c8f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9c8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c8f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-116">Not supported.</span></span>|
|<span data-ttu-id="b9c8f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9c8f-117">Application</span></span>|<span data-ttu-id="b9c8f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c8f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c8f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9c8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b9c8f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9c8f-120">Request headers</span></span>
|<span data-ttu-id="b9c8f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9c8f-121">Header</span></span>|<span data-ttu-id="b9c8f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9c8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c8f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9c8f-123">Authorization</span></span>|<span data-ttu-id="b9c8f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9c8f-125">Accept</span></span>|<span data-ttu-id="b9c8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c8f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9c8f-127">Request body</span></span>
<span data-ttu-id="b9c8f-128">В тексте запроса добавьте представление объекта Усераппинсталлстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="b9c8f-129">В следующей таблице приведены свойства, необходимые при создании Усераппинсталлстатус.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="b9c8f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9c8f-130">Property</span></span>|<span data-ttu-id="b9c8f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9c8f-131">Type</span></span>|<span data-ttu-id="b9c8f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c8f-133">id</span><span class="sxs-lookup"><span data-stu-id="b9c8f-133">id</span></span>|<span data-ttu-id="b9c8f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b9c8f-134">String</span></span>|<span data-ttu-id="b9c8f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-135">Key of the entity.</span></span>|
|<span data-ttu-id="b9c8f-136">userName</span><span class="sxs-lookup"><span data-stu-id="b9c8f-136">userName</span></span>|<span data-ttu-id="b9c8f-137">String</span><span class="sxs-lookup"><span data-stu-id="b9c8f-137">String</span></span>|<span data-ttu-id="b9c8f-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-138">User name.</span></span>|
|<span data-ttu-id="b9c8f-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9c8f-139">userPrincipalName</span></span>|<span data-ttu-id="b9c8f-140">String</span><span class="sxs-lookup"><span data-stu-id="b9c8f-140">String</span></span>|<span data-ttu-id="b9c8f-141">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-141">User Principal Name.</span></span>|
|<span data-ttu-id="b9c8f-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b9c8f-142">installedDeviceCount</span></span>|<span data-ttu-id="b9c8f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c8f-143">Int32</span></span>|<span data-ttu-id="b9c8f-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-144">Installed Device Count.</span></span>|
|<span data-ttu-id="b9c8f-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b9c8f-145">failedDeviceCount</span></span>|<span data-ttu-id="b9c8f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c8f-146">Int32</span></span>|<span data-ttu-id="b9c8f-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-147">Failed Device Count.</span></span>|
|<span data-ttu-id="b9c8f-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b9c8f-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="b9c8f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c8f-149">Int32</span></span>|<span data-ttu-id="b9c8f-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="b9c8f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c8f-151">Response</span></span>
<span data-ttu-id="b9c8f-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c8f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="b9c8f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c8f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9c8f-154">Request</span></span>
<span data-ttu-id="b9c8f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9c8f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c8f-156">Response</span></span>
<span data-ttu-id="b9c8f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9c8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





