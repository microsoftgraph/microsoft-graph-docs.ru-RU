---
title: Обновление userAppInstallStatus
description: Обновление свойства объекта userAppInstallStatus.
author: tfitzmac
ms.openlocfilehash: 7ce3ec17f443f90bd4d31df1ec0ee46269334b5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341533"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="081a6-103">Обновление userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="081a6-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="081a6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="081a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="081a6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="081a6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="081a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="081a6-107">Обновление свойства объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="081a6-107">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="081a6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="081a6-108">Prerequisites</span></span>
<span data-ttu-id="081a6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="081a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="081a6-111">Permission type</span></span>|<span data-ttu-id="081a6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="081a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="081a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="081a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="081a6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="081a6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="081a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="081a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="081a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a6-116">Not supported.</span></span>|
|<span data-ttu-id="081a6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="081a6-117">Application</span></span>|<span data-ttu-id="081a6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="081a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="081a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="081a6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="081a6-120">Request headers</span></span>
|<span data-ttu-id="081a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="081a6-121">Header</span></span>|<span data-ttu-id="081a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="081a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="081a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="081a6-123">Authorization</span></span>|<span data-ttu-id="081a6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="081a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="081a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="081a6-125">Accept</span></span>|<span data-ttu-id="081a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="081a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="081a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="081a6-127">Request body</span></span>
<span data-ttu-id="081a6-128">В тексте запроса укажите представление JSON для объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="081a6-128">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="081a6-129">В следующей таблице показаны свойства, которые необходимы для создания [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="081a6-129">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="081a6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="081a6-130">Property</span></span>|<span data-ttu-id="081a6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="081a6-131">Type</span></span>|<span data-ttu-id="081a6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="081a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="081a6-133">id</span><span class="sxs-lookup"><span data-stu-id="081a6-133">id</span></span>|<span data-ttu-id="081a6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="081a6-134">String</span></span>|<span data-ttu-id="081a6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="081a6-135">Key of the entity.</span></span>|
|<span data-ttu-id="081a6-136">userName</span><span class="sxs-lookup"><span data-stu-id="081a6-136">userName</span></span>|<span data-ttu-id="081a6-137">String</span><span class="sxs-lookup"><span data-stu-id="081a6-137">String</span></span>|<span data-ttu-id="081a6-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="081a6-138">User name.</span></span>|
|<span data-ttu-id="081a6-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="081a6-139">userPrincipalName</span></span>|<span data-ttu-id="081a6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="081a6-140">String</span></span>|<span data-ttu-id="081a6-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="081a6-141">User Principal Name.</span></span>|
|<span data-ttu-id="081a6-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="081a6-142">installedDeviceCount</span></span>|<span data-ttu-id="081a6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="081a6-143">Int32</span></span>|<span data-ttu-id="081a6-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="081a6-144">Installed Device Count.</span></span>|
|<span data-ttu-id="081a6-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="081a6-145">failedDeviceCount</span></span>|<span data-ttu-id="081a6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="081a6-146">Int32</span></span>|<span data-ttu-id="081a6-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="081a6-147">Failed Device Count.</span></span>|
|<span data-ttu-id="081a6-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="081a6-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="081a6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="081a6-149">Int32</span></span>|<span data-ttu-id="081a6-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="081a6-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="081a6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="081a6-151">Response</span></span>
<span data-ttu-id="081a6-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="081a6-152">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="081a6-153">Пример</span><span class="sxs-lookup"><span data-stu-id="081a6-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="081a6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="081a6-154">Request</span></span>
<span data-ttu-id="081a6-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="081a6-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 180

{
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="081a6-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="081a6-156">Response</span></span>
<span data-ttu-id="081a6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="081a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





