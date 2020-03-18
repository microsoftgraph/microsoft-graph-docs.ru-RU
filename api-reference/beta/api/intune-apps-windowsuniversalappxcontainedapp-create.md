---
title: Создание Виндовсуниверсалаппксконтаинедапп
description: Создание нового объекта Виндовсуниверсалаппксконтаинедапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e45f88ec15241bec5ee408563db26d02f4212233
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760643"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="4a180-103">Создание Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="4a180-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="4a180-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a180-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a180-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a180-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a180-106">Создание нового объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4a180-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a180-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a180-107">Prerequisites</span></span>
<span data-ttu-id="4a180-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a180-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a180-110">Permission type</span></span>|<span data-ttu-id="4a180-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a180-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a180-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a180-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a180-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a180-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a180-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a180-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a180-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a180-115">Not supported.</span></span>|
|<span data-ttu-id="4a180-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a180-116">Application</span></span>|<span data-ttu-id="4a180-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a180-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a180-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a180-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="4a180-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a180-119">Request headers</span></span>
|<span data-ttu-id="4a180-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a180-120">Header</span></span>|<span data-ttu-id="4a180-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a180-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a180-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a180-122">Authorization</span></span>|<span data-ttu-id="4a180-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a180-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a180-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a180-124">Accept</span></span>|<span data-ttu-id="4a180-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a180-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a180-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a180-126">Request body</span></span>
<span data-ttu-id="4a180-127">В тексте запроса добавьте представление объекта Виндовсуниверсалаппксконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a180-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="4a180-128">В следующей таблице приведены свойства, необходимые при создании Виндовсуниверсалаппксконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="4a180-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="4a180-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a180-129">Property</span></span>|<span data-ttu-id="4a180-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a180-130">Type</span></span>|<span data-ttu-id="4a180-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a180-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a180-132">id</span><span class="sxs-lookup"><span data-stu-id="4a180-132">id</span></span>|<span data-ttu-id="4a180-133">String</span><span class="sxs-lookup"><span data-stu-id="4a180-133">String</span></span>|<span data-ttu-id="4a180-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4a180-134">Key of the entity.</span></span> <span data-ttu-id="4a180-135">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a180-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="4a180-136">Модели</span><span class="sxs-lookup"><span data-stu-id="4a180-136">appUserModelId</span></span>|<span data-ttu-id="4a180-137">String</span><span class="sxs-lookup"><span data-stu-id="4a180-137">String</span></span>|<span data-ttu-id="4a180-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="4a180-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="4a180-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a180-139">Response</span></span>
<span data-ttu-id="4a180-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a180-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a180-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4a180-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a180-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a180-142">Request</span></span>
<span data-ttu-id="4a180-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a180-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="4a180-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a180-144">Response</span></span>
<span data-ttu-id="4a180-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a180-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




