---
title: Создание userAppInstallStatus
description: Создание нового объекта userAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ebb03db9e8d9f0c2eab30ecebbee4dbf8832654
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397871"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="08847-103">Создание userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="08847-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="08847-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08847-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08847-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08847-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08847-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08847-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08847-107">Создание нового объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="08847-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08847-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="08847-108">Prerequisites</span></span>
<span data-ttu-id="08847-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08847-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08847-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08847-111">Permission type</span></span>|<span data-ttu-id="08847-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08847-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08847-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08847-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08847-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08847-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08847-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08847-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08847-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08847-116">Not supported.</span></span>|
|<span data-ttu-id="08847-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08847-117">Application</span></span>|<span data-ttu-id="08847-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08847-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08847-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08847-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="08847-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08847-120">Request headers</span></span>
|<span data-ttu-id="08847-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08847-121">Header</span></span>|<span data-ttu-id="08847-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08847-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08847-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08847-123">Authorization</span></span>|<span data-ttu-id="08847-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08847-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08847-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08847-125">Accept</span></span>|<span data-ttu-id="08847-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08847-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08847-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08847-127">Request body</span></span>
<span data-ttu-id="08847-128">В тексте запроса укажите представление JSON для объекта userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="08847-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="08847-129">В следующей таблице показаны свойства, которые необходимы для создания userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="08847-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="08847-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08847-130">Property</span></span>|<span data-ttu-id="08847-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08847-131">Type</span></span>|<span data-ttu-id="08847-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08847-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08847-133">id</span><span class="sxs-lookup"><span data-stu-id="08847-133">id</span></span>|<span data-ttu-id="08847-134">String</span><span class="sxs-lookup"><span data-stu-id="08847-134">String</span></span>|<span data-ttu-id="08847-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08847-135">Key of the entity.</span></span>|
|<span data-ttu-id="08847-136">userName</span><span class="sxs-lookup"><span data-stu-id="08847-136">userName</span></span>|<span data-ttu-id="08847-137">String</span><span class="sxs-lookup"><span data-stu-id="08847-137">String</span></span>|<span data-ttu-id="08847-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="08847-138">User name.</span></span>|
|<span data-ttu-id="08847-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08847-139">userPrincipalName</span></span>|<span data-ttu-id="08847-140">String</span><span class="sxs-lookup"><span data-stu-id="08847-140">String</span></span>|<span data-ttu-id="08847-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="08847-141">User Principal Name.</span></span>|
|<span data-ttu-id="08847-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08847-142">installedDeviceCount</span></span>|<span data-ttu-id="08847-143">Int32</span><span class="sxs-lookup"><span data-stu-id="08847-143">Int32</span></span>|<span data-ttu-id="08847-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="08847-144">Installed Device Count.</span></span>|
|<span data-ttu-id="08847-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08847-145">failedDeviceCount</span></span>|<span data-ttu-id="08847-146">Int32</span><span class="sxs-lookup"><span data-stu-id="08847-146">Int32</span></span>|<span data-ttu-id="08847-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="08847-147">Failed Device Count.</span></span>|
|<span data-ttu-id="08847-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08847-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="08847-149">Int32</span><span class="sxs-lookup"><span data-stu-id="08847-149">Int32</span></span>|<span data-ttu-id="08847-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="08847-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="08847-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="08847-151">Response</span></span>
<span data-ttu-id="08847-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08847-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08847-153">Пример</span><span class="sxs-lookup"><span data-stu-id="08847-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="08847-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="08847-154">Request</span></span>
<span data-ttu-id="08847-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08847-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08847-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="08847-156">Response</span></span>
<span data-ttu-id="08847-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08847-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




