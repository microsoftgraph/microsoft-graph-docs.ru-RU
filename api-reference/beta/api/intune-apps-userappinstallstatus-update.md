---
title: Обновление userAppInstallStatus
description: Обновление свойства объекта userAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 237e9f28f36fb25ea5ddad46f5a6a75242767c6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413838"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="4e22c-103">Обновление userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="4e22c-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="4e22c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e22c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e22c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e22c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e22c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e22c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e22c-107">Обновление свойства объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4e22c-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e22c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4e22c-108">Prerequisites</span></span>
<span data-ttu-id="4e22c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e22c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e22c-111">Permission type</span></span>|<span data-ttu-id="4e22c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e22c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e22c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e22c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e22c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e22c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e22c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e22c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e22c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e22c-116">Not supported.</span></span>|
|<span data-ttu-id="4e22c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e22c-117">Application</span></span>|<span data-ttu-id="4e22c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e22c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e22c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e22c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4e22c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e22c-120">Request headers</span></span>
|<span data-ttu-id="4e22c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e22c-121">Header</span></span>|<span data-ttu-id="4e22c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e22c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e22c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e22c-123">Authorization</span></span>|<span data-ttu-id="4e22c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e22c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e22c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e22c-125">Accept</span></span>|<span data-ttu-id="4e22c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e22c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e22c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e22c-127">Request body</span></span>
<span data-ttu-id="4e22c-128">В тексте запроса укажите представление JSON для объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4e22c-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="4e22c-129">В следующей таблице показаны свойства, которые необходимы для создания [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4e22c-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="4e22c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e22c-130">Property</span></span>|<span data-ttu-id="4e22c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e22c-131">Type</span></span>|<span data-ttu-id="4e22c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e22c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e22c-133">id</span><span class="sxs-lookup"><span data-stu-id="4e22c-133">id</span></span>|<span data-ttu-id="4e22c-134">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-134">String</span></span>|<span data-ttu-id="4e22c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e22c-135">Key of the entity.</span></span>|
|<span data-ttu-id="4e22c-136">userName</span><span class="sxs-lookup"><span data-stu-id="4e22c-136">userName</span></span>|<span data-ttu-id="4e22c-137">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-137">String</span></span>|<span data-ttu-id="4e22c-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4e22c-138">User name.</span></span>|
|<span data-ttu-id="4e22c-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e22c-139">userPrincipalName</span></span>|<span data-ttu-id="4e22c-140">String</span><span class="sxs-lookup"><span data-stu-id="4e22c-140">String</span></span>|<span data-ttu-id="4e22c-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="4e22c-141">User Principal Name.</span></span>|
|<span data-ttu-id="4e22c-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e22c-142">installedDeviceCount</span></span>|<span data-ttu-id="4e22c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4e22c-143">Int32</span></span>|<span data-ttu-id="4e22c-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4e22c-144">Installed Device Count.</span></span>|
|<span data-ttu-id="4e22c-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e22c-145">failedDeviceCount</span></span>|<span data-ttu-id="4e22c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4e22c-146">Int32</span></span>|<span data-ttu-id="4e22c-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4e22c-147">Failed Device Count.</span></span>|
|<span data-ttu-id="4e22c-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e22c-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="4e22c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4e22c-149">Int32</span></span>|<span data-ttu-id="4e22c-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4e22c-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="4e22c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e22c-151">Response</span></span>
<span data-ttu-id="4e22c-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4e22c-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e22c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4e22c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e22c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e22c-154">Request</span></span>
<span data-ttu-id="4e22c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e22c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e22c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e22c-156">Response</span></span>
<span data-ttu-id="4e22c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e22c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




