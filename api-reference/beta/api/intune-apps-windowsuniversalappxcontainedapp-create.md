---
title: Создание Виндовсуниверсалаппксконтаинедапп
description: Создание нового объекта Виндовсуниверсалаппксконтаинедапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 751808f3a63bfca7fd9ab56e39752f0631f98c71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976020"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="d1916-103">Создание Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="d1916-103">Create windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="d1916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1916-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1916-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1916-107">Создание нового объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d1916-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1916-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1916-108">Prerequisites</span></span>
<span data-ttu-id="d1916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1916-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1916-111">Permission type</span></span>|<span data-ttu-id="d1916-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1916-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1916-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1916-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1916-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1916-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1916-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1916-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1916-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1916-116">Not supported.</span></span>|
|<span data-ttu-id="d1916-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1916-117">Application</span></span>|<span data-ttu-id="d1916-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1916-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1916-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1916-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="d1916-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1916-120">Request headers</span></span>
|<span data-ttu-id="d1916-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1916-121">Header</span></span>|<span data-ttu-id="d1916-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1916-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1916-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1916-123">Authorization</span></span>|<span data-ttu-id="d1916-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1916-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1916-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1916-125">Accept</span></span>|<span data-ttu-id="d1916-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1916-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1916-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1916-127">Request body</span></span>
<span data-ttu-id="d1916-128">В тексте запроса добавьте представление объекта Виндовсуниверсалаппксконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1916-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="d1916-129">В следующей таблице приведены свойства, необходимые при создании Виндовсуниверсалаппксконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="d1916-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="d1916-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1916-130">Property</span></span>|<span data-ttu-id="d1916-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1916-131">Type</span></span>|<span data-ttu-id="d1916-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1916-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1916-133">id</span><span class="sxs-lookup"><span data-stu-id="d1916-133">id</span></span>|<span data-ttu-id="d1916-134">String</span><span class="sxs-lookup"><span data-stu-id="d1916-134">String</span></span>|<span data-ttu-id="d1916-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d1916-135">Key of the entity.</span></span> <span data-ttu-id="d1916-136">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d1916-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="d1916-137">Модели</span><span class="sxs-lookup"><span data-stu-id="d1916-137">appUserModelId</span></span>|<span data-ttu-id="d1916-138">String</span><span class="sxs-lookup"><span data-stu-id="d1916-138">String</span></span>|<span data-ttu-id="d1916-139">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="d1916-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="d1916-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1916-140">Response</span></span>
<span data-ttu-id="d1916-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1916-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1916-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d1916-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1916-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1916-143">Request</span></span>
<span data-ttu-id="d1916-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1916-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="d1916-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1916-145">Response</span></span>
<span data-ttu-id="d1916-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1916-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






