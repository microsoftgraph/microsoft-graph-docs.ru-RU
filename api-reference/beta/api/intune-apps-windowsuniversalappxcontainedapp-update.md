---
title: Обновление Виндовсуниверсалаппксконтаинедапп
description: Обновление свойств объекта Виндовсуниверсалаппксконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a3bacf74734fefe8255da981f0f71f4389db610
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159838"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="c1b32-103">Обновление Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="c1b32-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="c1b32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1b32-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1b32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1b32-106">Обновление свойств объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c1b32-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1b32-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1b32-107">Prerequisites</span></span>
<span data-ttu-id="c1b32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1b32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1b32-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b32-110">Permission type</span></span>|<span data-ttu-id="c1b32-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1b32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b32-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1b32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b32-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1b32-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1b32-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1b32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b32-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b32-115">Not supported.</span></span>|
|<span data-ttu-id="c1b32-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1b32-116">Application</span></span>|<span data-ttu-id="c1b32-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b32-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1b32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c1b32-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1b32-119">Request headers</span></span>
|<span data-ttu-id="c1b32-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1b32-120">Header</span></span>|<span data-ttu-id="c1b32-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1b32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b32-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1b32-122">Authorization</span></span>|<span data-ttu-id="c1b32-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c1b32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b32-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1b32-124">Accept</span></span>|<span data-ttu-id="c1b32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b32-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1b32-126">Request body</span></span>
<span data-ttu-id="c1b32-127">В тексте запроса добавьте представление объекта [Виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1b32-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="c1b32-128">В следующей таблице приведены свойства, необходимые при создании [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1b32-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="c1b32-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1b32-129">Property</span></span>|<span data-ttu-id="c1b32-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c1b32-130">Type</span></span>|<span data-ttu-id="c1b32-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c1b32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1b32-132">id</span><span class="sxs-lookup"><span data-stu-id="c1b32-132">id</span></span>|<span data-ttu-id="c1b32-133">String</span><span class="sxs-lookup"><span data-stu-id="c1b32-133">String</span></span>|<span data-ttu-id="c1b32-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1b32-134">Key of the entity.</span></span> <span data-ttu-id="c1b32-135">НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1b32-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c1b32-136">Модели</span><span class="sxs-lookup"><span data-stu-id="c1b32-136">appUserModelId</span></span>|<span data-ttu-id="c1b32-137">String</span><span class="sxs-lookup"><span data-stu-id="c1b32-137">String</span></span>|<span data-ttu-id="c1b32-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="c1b32-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="c1b32-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b32-139">Response</span></span>
<span data-ttu-id="c1b32-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1b32-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b32-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c1b32-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1b32-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b32-142">Request</span></span>
<span data-ttu-id="c1b32-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1b32-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c1b32-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b32-144">Response</span></span>
<span data-ttu-id="c1b32-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




