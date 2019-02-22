---
title: Создание Виндовсуниверсалаппксконтаинедапп
description: Создание нового объекта Виндовсуниверсалаппксконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72e171d4a967b9b8dcc7a5271ba09c2afe8c6744
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164857"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="8e95f-103">Создание Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="8e95f-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="8e95f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e95f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e95f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e95f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e95f-106">Создание нового объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8e95f-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e95f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e95f-107">Prerequisites</span></span>
<span data-ttu-id="8e95f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e95f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e95f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e95f-110">Permission type</span></span>|<span data-ttu-id="8e95f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e95f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e95f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e95f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e95f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e95f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e95f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e95f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e95f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e95f-115">Not supported.</span></span>|
|<span data-ttu-id="8e95f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e95f-116">Application</span></span>|<span data-ttu-id="8e95f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e95f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e95f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e95f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="8e95f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e95f-119">Request headers</span></span>
|<span data-ttu-id="8e95f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e95f-120">Header</span></span>|<span data-ttu-id="8e95f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8e95f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e95f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e95f-122">Authorization</span></span>|<span data-ttu-id="8e95f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e95f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e95f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8e95f-124">Accept</span></span>|<span data-ttu-id="8e95f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e95f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e95f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e95f-126">Request body</span></span>
<span data-ttu-id="8e95f-127">В тексте запроса добавьте представление объекта Виндовсуниверсалаппксконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e95f-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="8e95f-128">В следующей таблице приведены свойства, необходимые при создании Виндовсуниверсалаппксконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="8e95f-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="8e95f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e95f-129">Property</span></span>|<span data-ttu-id="8e95f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8e95f-130">Type</span></span>|<span data-ttu-id="8e95f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8e95f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e95f-132">id</span><span class="sxs-lookup"><span data-stu-id="8e95f-132">id</span></span>|<span data-ttu-id="8e95f-133">String</span><span class="sxs-lookup"><span data-stu-id="8e95f-133">String</span></span>|<span data-ttu-id="8e95f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e95f-134">Key of the entity.</span></span> <span data-ttu-id="8e95f-135">НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e95f-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="8e95f-136">Модели</span><span class="sxs-lookup"><span data-stu-id="8e95f-136">appUserModelId</span></span>|<span data-ttu-id="8e95f-137">String</span><span class="sxs-lookup"><span data-stu-id="8e95f-137">String</span></span>|<span data-ttu-id="8e95f-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="8e95f-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="8e95f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e95f-139">Response</span></span>
<span data-ttu-id="8e95f-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e95f-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e95f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8e95f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e95f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e95f-142">Request</span></span>
<span data-ttu-id="8e95f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e95f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="8e95f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e95f-144">Response</span></span>
<span data-ttu-id="8e95f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e95f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




