---
title: Создание userAppInstallStatus
description: Создание нового объекта userAppInstallStatus.
author: tfitzmac
ms.openlocfilehash: ef110f5ce911e7e2244ebe2a50bcad194421ecea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308486"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="01074-103">Создание userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="01074-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="01074-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01074-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01074-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01074-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01074-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01074-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01074-107">Создание нового объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="01074-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01074-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01074-108">Prerequisites</span></span>
<span data-ttu-id="01074-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01074-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01074-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01074-111">Permission type</span></span>|<span data-ttu-id="01074-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01074-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01074-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01074-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01074-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01074-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01074-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01074-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01074-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01074-116">Not supported.</span></span>|
|<span data-ttu-id="01074-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01074-117">Application</span></span>|<span data-ttu-id="01074-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01074-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01074-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01074-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="01074-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01074-120">Request headers</span></span>
|<span data-ttu-id="01074-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01074-121">Header</span></span>|<span data-ttu-id="01074-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01074-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01074-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01074-123">Authorization</span></span>|<span data-ttu-id="01074-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01074-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01074-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01074-125">Accept</span></span>|<span data-ttu-id="01074-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01074-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01074-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01074-127">Request body</span></span>
<span data-ttu-id="01074-128">В тексте запроса укажите представление JSON для объекта userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="01074-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="01074-129">В следующей таблице показаны свойства, которые необходимы для создания userAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="01074-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="01074-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01074-130">Property</span></span>|<span data-ttu-id="01074-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01074-131">Type</span></span>|<span data-ttu-id="01074-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01074-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01074-133">id</span><span class="sxs-lookup"><span data-stu-id="01074-133">id</span></span>|<span data-ttu-id="01074-134">Строка</span><span class="sxs-lookup"><span data-stu-id="01074-134">String</span></span>|<span data-ttu-id="01074-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01074-135">Key of the entity.</span></span>|
|<span data-ttu-id="01074-136">userName</span><span class="sxs-lookup"><span data-stu-id="01074-136">userName</span></span>|<span data-ttu-id="01074-137">String</span><span class="sxs-lookup"><span data-stu-id="01074-137">String</span></span>|<span data-ttu-id="01074-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="01074-138">User name.</span></span>|
|<span data-ttu-id="01074-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="01074-139">userPrincipalName</span></span>|<span data-ttu-id="01074-140">Строка</span><span class="sxs-lookup"><span data-stu-id="01074-140">String</span></span>|<span data-ttu-id="01074-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="01074-141">User Principal Name.</span></span>|
|<span data-ttu-id="01074-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01074-142">installedDeviceCount</span></span>|<span data-ttu-id="01074-143">Int32</span><span class="sxs-lookup"><span data-stu-id="01074-143">Int32</span></span>|<span data-ttu-id="01074-144">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="01074-144">Installed Device Count.</span></span>|
|<span data-ttu-id="01074-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01074-145">failedDeviceCount</span></span>|<span data-ttu-id="01074-146">Int32</span><span class="sxs-lookup"><span data-stu-id="01074-146">Int32</span></span>|<span data-ttu-id="01074-147">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="01074-147">Failed Device Count.</span></span>|
|<span data-ttu-id="01074-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01074-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="01074-149">Int32</span><span class="sxs-lookup"><span data-stu-id="01074-149">Int32</span></span>|<span data-ttu-id="01074-150">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="01074-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="01074-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="01074-151">Response</span></span>
<span data-ttu-id="01074-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01074-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01074-153">Пример</span><span class="sxs-lookup"><span data-stu-id="01074-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="01074-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="01074-154">Request</span></span>
<span data-ttu-id="01074-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01074-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01074-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="01074-156">Response</span></span>
<span data-ttu-id="01074-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01074-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





