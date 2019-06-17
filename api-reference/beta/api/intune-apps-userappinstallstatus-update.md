---
title: Обновление Усераппинсталлстатус
description: Обновление свойств объекта Усераппинсталлстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fdbc155fb82b89520cd78b5aa72236cc4f44ba71
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973371"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="37e60-103">Обновление Усераппинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="37e60-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="37e60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37e60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37e60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e60-106">Обновление свойств объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="37e60-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37e60-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37e60-107">Prerequisites</span></span>
<span data-ttu-id="37e60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37e60-110">Permission type</span></span>|<span data-ttu-id="37e60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37e60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37e60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37e60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37e60-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e60-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37e60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37e60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e60-115">Not supported.</span></span>|
|<span data-ttu-id="37e60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37e60-116">Application</span></span>|<span data-ttu-id="37e60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37e60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37e60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="37e60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37e60-119">Request headers</span></span>
|<span data-ttu-id="37e60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37e60-120">Header</span></span>|<span data-ttu-id="37e60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37e60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37e60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37e60-122">Authorization</span></span>|<span data-ttu-id="37e60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37e60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37e60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37e60-124">Accept</span></span>|<span data-ttu-id="37e60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37e60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37e60-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37e60-126">Request body</span></span>
<span data-ttu-id="37e60-127">В тексте запроса добавьте представление объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37e60-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="37e60-128">В следующей таблице приведены свойства, необходимые при создании [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="37e60-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="37e60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37e60-129">Property</span></span>|<span data-ttu-id="37e60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37e60-130">Type</span></span>|<span data-ttu-id="37e60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37e60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e60-132">id</span><span class="sxs-lookup"><span data-stu-id="37e60-132">id</span></span>|<span data-ttu-id="37e60-133">Строка</span><span class="sxs-lookup"><span data-stu-id="37e60-133">String</span></span>|<span data-ttu-id="37e60-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37e60-134">Key of the entity.</span></span>|
|<span data-ttu-id="37e60-135">userName</span><span class="sxs-lookup"><span data-stu-id="37e60-135">userName</span></span>|<span data-ttu-id="37e60-136">String</span><span class="sxs-lookup"><span data-stu-id="37e60-136">String</span></span>|<span data-ttu-id="37e60-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="37e60-137">User name.</span></span>|
|<span data-ttu-id="37e60-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37e60-138">userPrincipalName</span></span>|<span data-ttu-id="37e60-139">String</span><span class="sxs-lookup"><span data-stu-id="37e60-139">String</span></span>|<span data-ttu-id="37e60-140">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="37e60-140">User Principal Name.</span></span>|
|<span data-ttu-id="37e60-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37e60-141">installedDeviceCount</span></span>|<span data-ttu-id="37e60-142">Int32</span><span class="sxs-lookup"><span data-stu-id="37e60-142">Int32</span></span>|<span data-ttu-id="37e60-143">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="37e60-143">Installed Device Count.</span></span>|
|<span data-ttu-id="37e60-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37e60-144">failedDeviceCount</span></span>|<span data-ttu-id="37e60-145">Int32</span><span class="sxs-lookup"><span data-stu-id="37e60-145">Int32</span></span>|<span data-ttu-id="37e60-146">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="37e60-146">Failed Device Count.</span></span>|
|<span data-ttu-id="37e60-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37e60-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="37e60-148">Int32</span><span class="sxs-lookup"><span data-stu-id="37e60-148">Int32</span></span>|<span data-ttu-id="37e60-149">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="37e60-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="37e60-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="37e60-150">Response</span></span>
<span data-ttu-id="37e60-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37e60-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e60-152">Пример</span><span class="sxs-lookup"><span data-stu-id="37e60-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="37e60-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="37e60-153">Request</span></span>
<span data-ttu-id="37e60-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37e60-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37e60-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="37e60-155">Response</span></span>
<span data-ttu-id="37e60-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37e60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





