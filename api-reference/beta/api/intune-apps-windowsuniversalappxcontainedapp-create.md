---
title: Создание Виндовсуниверсалаппксконтаинедапп
description: Создание нового объекта Виндовсуниверсалаппксконтаинедапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e80322df3ab56d087b29d17c0720445a05fca49
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727901"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="939bf-103">Создание Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="939bf-103">Create windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="939bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="939bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="939bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="939bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="939bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="939bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="939bf-107">Создание нового объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="939bf-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="939bf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="939bf-108">Prerequisites</span></span>
<span data-ttu-id="939bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="939bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="939bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="939bf-111">Permission type</span></span>|<span data-ttu-id="939bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="939bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="939bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="939bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="939bf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="939bf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="939bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="939bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="939bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="939bf-116">Not supported.</span></span>|
|<span data-ttu-id="939bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="939bf-117">Application</span></span>|<span data-ttu-id="939bf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="939bf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="939bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="939bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="939bf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="939bf-120">Request headers</span></span>
|<span data-ttu-id="939bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="939bf-121">Header</span></span>|<span data-ttu-id="939bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="939bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="939bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="939bf-123">Authorization</span></span>|<span data-ttu-id="939bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="939bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="939bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="939bf-125">Accept</span></span>|<span data-ttu-id="939bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="939bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="939bf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="939bf-127">Request body</span></span>
<span data-ttu-id="939bf-128">В тексте запроса добавьте представление объекта Виндовсуниверсалаппксконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="939bf-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="939bf-129">В следующей таблице приведены свойства, необходимые при создании Виндовсуниверсалаппксконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="939bf-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="939bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="939bf-130">Property</span></span>|<span data-ttu-id="939bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="939bf-131">Type</span></span>|<span data-ttu-id="939bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="939bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="939bf-133">id</span><span class="sxs-lookup"><span data-stu-id="939bf-133">id</span></span>|<span data-ttu-id="939bf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="939bf-134">String</span></span>|<span data-ttu-id="939bf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="939bf-135">Key of the entity.</span></span> <span data-ttu-id="939bf-136">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="939bf-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="939bf-137">Модели</span><span class="sxs-lookup"><span data-stu-id="939bf-137">appUserModelId</span></span>|<span data-ttu-id="939bf-138">Строка</span><span class="sxs-lookup"><span data-stu-id="939bf-138">String</span></span>|<span data-ttu-id="939bf-139">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="939bf-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="939bf-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="939bf-140">Response</span></span>
<span data-ttu-id="939bf-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="939bf-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="939bf-142">Пример</span><span class="sxs-lookup"><span data-stu-id="939bf-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="939bf-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="939bf-143">Request</span></span>
<span data-ttu-id="939bf-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="939bf-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="939bf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="939bf-145">Response</span></span>
<span data-ttu-id="939bf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="939bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





