---
title: Обновление Усераппинсталлстатус
description: Обновление свойств объекта Усераппинсталлстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aea00e27c59e88ad622ca8c88bf4de7727ce7e81
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328881"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="19fc6-103">Обновление Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="19fc6-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="19fc6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19fc6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19fc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fc6-106">Обновление свойств объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="19fc6-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19fc6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19fc6-107">Prerequisites</span></span>
<span data-ttu-id="19fc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19fc6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19fc6-110">Permission type</span></span>|<span data-ttu-id="19fc6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19fc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19fc6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19fc6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19fc6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fc6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19fc6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19fc6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19fc6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fc6-115">Not supported.</span></span>|
|<span data-ttu-id="19fc6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19fc6-116">Application</span></span>|<span data-ttu-id="19fc6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fc6-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fc6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19fc6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="19fc6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19fc6-119">Request headers</span></span>
|<span data-ttu-id="19fc6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19fc6-120">Header</span></span>|<span data-ttu-id="19fc6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19fc6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19fc6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19fc6-122">Authorization</span></span>|<span data-ttu-id="19fc6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19fc6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19fc6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19fc6-124">Accept</span></span>|<span data-ttu-id="19fc6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19fc6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fc6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19fc6-126">Request body</span></span>
<span data-ttu-id="19fc6-127">В тексте запроса добавьте представление объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19fc6-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="19fc6-128">В следующей таблице приведены свойства, необходимые при создании [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="19fc6-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="19fc6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="19fc6-129">Property</span></span>|<span data-ttu-id="19fc6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="19fc6-130">Type</span></span>|<span data-ttu-id="19fc6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="19fc6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fc6-132">id</span><span class="sxs-lookup"><span data-stu-id="19fc6-132">id</span></span>|<span data-ttu-id="19fc6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="19fc6-133">String</span></span>|<span data-ttu-id="19fc6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19fc6-134">Key of the entity.</span></span>|
|<span data-ttu-id="19fc6-135">userName</span><span class="sxs-lookup"><span data-stu-id="19fc6-135">userName</span></span>|<span data-ttu-id="19fc6-136">String</span><span class="sxs-lookup"><span data-stu-id="19fc6-136">String</span></span>|<span data-ttu-id="19fc6-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="19fc6-137">User name.</span></span>|
|<span data-ttu-id="19fc6-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19fc6-138">userPrincipalName</span></span>|<span data-ttu-id="19fc6-139">String</span><span class="sxs-lookup"><span data-stu-id="19fc6-139">String</span></span>|<span data-ttu-id="19fc6-140">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="19fc6-140">User Principal Name.</span></span>|
|<span data-ttu-id="19fc6-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19fc6-141">installedDeviceCount</span></span>|<span data-ttu-id="19fc6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="19fc6-142">Int32</span></span>|<span data-ttu-id="19fc6-143">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="19fc6-143">Installed Device Count.</span></span>|
|<span data-ttu-id="19fc6-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19fc6-144">failedDeviceCount</span></span>|<span data-ttu-id="19fc6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="19fc6-145">Int32</span></span>|<span data-ttu-id="19fc6-146">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="19fc6-146">Failed Device Count.</span></span>|
|<span data-ttu-id="19fc6-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19fc6-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="19fc6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="19fc6-148">Int32</span></span>|<span data-ttu-id="19fc6-149">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="19fc6-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="19fc6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="19fc6-150">Response</span></span>
<span data-ttu-id="19fc6-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19fc6-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fc6-152">Пример</span><span class="sxs-lookup"><span data-stu-id="19fc6-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fc6-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="19fc6-153">Request</span></span>
<span data-ttu-id="19fc6-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19fc6-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19fc6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="19fc6-155">Response</span></span>
<span data-ttu-id="19fc6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19fc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






