---
title: Создание Усераппинсталлстатус
description: Создание нового объекта Усераппинсталлстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 345650c5499959a57ede61605b00013d1d079866
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172256"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="f7e17-103">Создание Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="f7e17-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="f7e17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7e17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7e17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7e17-106">Создание нового объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="f7e17-106">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7e17-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7e17-107">Prerequisites</span></span>
<span data-ttu-id="f7e17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e17-110">Permission type</span></span>|<span data-ttu-id="f7e17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7e17-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e17-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7e17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e17-115">Not supported.</span></span>|
|<span data-ttu-id="f7e17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e17-116">Application</span></span>|<span data-ttu-id="f7e17-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e17-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7e17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f7e17-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e17-119">Request headers</span></span>
|<span data-ttu-id="f7e17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7e17-120">Header</span></span>|<span data-ttu-id="f7e17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f7e17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7e17-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7e17-122">Authorization</span></span>|<span data-ttu-id="f7e17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7e17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f7e17-124">Accept</span></span>|<span data-ttu-id="f7e17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7e17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e17-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7e17-126">Request body</span></span>
<span data-ttu-id="f7e17-127">В тексте запроса добавьте представление объекта Усераппинсталлстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7e17-127">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="f7e17-128">В следующей таблице приведены свойства, необходимые при создании Усераппинсталлстатус.</span><span class="sxs-lookup"><span data-stu-id="f7e17-128">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="f7e17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7e17-129">Property</span></span>|<span data-ttu-id="f7e17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e17-130">Type</span></span>|<span data-ttu-id="f7e17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7e17-132">id</span><span class="sxs-lookup"><span data-stu-id="f7e17-132">id</span></span>|<span data-ttu-id="f7e17-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f7e17-133">String</span></span>|<span data-ttu-id="f7e17-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7e17-134">Key of the entity.</span></span>|
|<span data-ttu-id="f7e17-135">userName</span><span class="sxs-lookup"><span data-stu-id="f7e17-135">userName</span></span>|<span data-ttu-id="f7e17-136">String</span><span class="sxs-lookup"><span data-stu-id="f7e17-136">String</span></span>|<span data-ttu-id="f7e17-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7e17-137">User name.</span></span>|
|<span data-ttu-id="f7e17-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7e17-138">userPrincipalName</span></span>|<span data-ttu-id="f7e17-139">String</span><span class="sxs-lookup"><span data-stu-id="f7e17-139">String</span></span>|<span data-ttu-id="f7e17-140">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7e17-140">User Principal Name.</span></span>|
|<span data-ttu-id="f7e17-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7e17-141">installedDeviceCount</span></span>|<span data-ttu-id="f7e17-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e17-142">Int32</span></span>|<span data-ttu-id="f7e17-143">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f7e17-143">Installed Device Count.</span></span>|
|<span data-ttu-id="f7e17-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7e17-144">failedDeviceCount</span></span>|<span data-ttu-id="f7e17-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e17-145">Int32</span></span>|<span data-ttu-id="f7e17-146">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="f7e17-146">Failed Device Count.</span></span>|
|<span data-ttu-id="f7e17-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7e17-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="f7e17-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e17-148">Int32</span></span>|<span data-ttu-id="f7e17-149">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f7e17-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f7e17-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e17-150">Response</span></span>
<span data-ttu-id="f7e17-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e17-151">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e17-152">Пример</span><span class="sxs-lookup"><span data-stu-id="f7e17-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7e17-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e17-153">Request</span></span>
<span data-ttu-id="f7e17-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7e17-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7e17-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e17-155">Response</span></span>
<span data-ttu-id="f7e17-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7e17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




