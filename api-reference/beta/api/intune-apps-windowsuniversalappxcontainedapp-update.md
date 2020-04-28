---
title: Обновление Виндовсуниверсалаппксконтаинедапп
description: Обновление свойств объекта Виндовсуниверсалаппксконтаинедапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30046e27c57f7a612919f591b971f9c0c3d41a32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393033"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="5e773-103">Обновление Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="5e773-103">Update windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="5e773-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e773-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e773-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e773-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e773-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e773-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e773-107">Обновление свойств объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5e773-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e773-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e773-108">Prerequisites</span></span>
<span data-ttu-id="5e773-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e773-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e773-111">Permission type</span></span>|<span data-ttu-id="5e773-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e773-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e773-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e773-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e773-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e773-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e773-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e773-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e773-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e773-116">Not supported.</span></span>|
|<span data-ttu-id="5e773-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e773-117">Application</span></span>|<span data-ttu-id="5e773-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e773-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e773-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e773-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5e773-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e773-120">Request headers</span></span>
|<span data-ttu-id="5e773-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e773-121">Header</span></span>|<span data-ttu-id="5e773-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e773-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e773-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e773-123">Authorization</span></span>|<span data-ttu-id="5e773-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e773-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e773-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e773-125">Accept</span></span>|<span data-ttu-id="5e773-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e773-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e773-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e773-127">Request body</span></span>
<span data-ttu-id="5e773-128">В тексте запроса добавьте представление объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e773-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="5e773-129">В следующей таблице приведены свойства, необходимые при создании [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="5e773-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="5e773-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e773-130">Property</span></span>|<span data-ttu-id="5e773-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e773-131">Type</span></span>|<span data-ttu-id="5e773-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e773-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e773-133">id</span><span class="sxs-lookup"><span data-stu-id="5e773-133">id</span></span>|<span data-ttu-id="5e773-134">String</span><span class="sxs-lookup"><span data-stu-id="5e773-134">String</span></span>|<span data-ttu-id="5e773-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e773-135">Key of the entity.</span></span> <span data-ttu-id="5e773-136">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5e773-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="5e773-137">Модели</span><span class="sxs-lookup"><span data-stu-id="5e773-137">appUserModelId</span></span>|<span data-ttu-id="5e773-138">String</span><span class="sxs-lookup"><span data-stu-id="5e773-138">String</span></span>|<span data-ttu-id="5e773-139">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="5e773-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="5e773-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e773-140">Response</span></span>
<span data-ttu-id="5e773-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e773-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e773-142">Пример</span><span class="sxs-lookup"><span data-stu-id="5e773-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e773-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e773-143">Request</span></span>
<span data-ttu-id="5e773-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e773-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="5e773-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e773-145">Response</span></span>
<span data-ttu-id="5e773-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e773-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```



