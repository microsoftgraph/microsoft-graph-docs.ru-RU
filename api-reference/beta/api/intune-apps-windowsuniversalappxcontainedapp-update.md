---
title: Обновление Виндовсуниверсалаппксконтаинедапп
description: Обновление свойств объекта Виндовсуниверсалаппксконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffc389f5b43132c21bfd0abfbfb7d45783e4ba75
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32485504"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="d29fd-103">Обновление Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="d29fd-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="d29fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d29fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d29fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d29fd-106">Обновление свойств объекта [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d29fd-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d29fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d29fd-107">Prerequisites</span></span>
<span data-ttu-id="d29fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d29fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d29fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d29fd-110">Permission type</span></span>|<span data-ttu-id="d29fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d29fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d29fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d29fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d29fd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d29fd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d29fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d29fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d29fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29fd-115">Not supported.</span></span>|
|<span data-ttu-id="d29fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d29fd-116">Application</span></span>|<span data-ttu-id="d29fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d29fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d29fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d29fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d29fd-119">Request headers</span></span>
|<span data-ttu-id="d29fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d29fd-120">Header</span></span>|<span data-ttu-id="d29fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d29fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d29fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d29fd-122">Authorization</span></span>|<span data-ttu-id="d29fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d29fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d29fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d29fd-124">Accept</span></span>|<span data-ttu-id="d29fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d29fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d29fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d29fd-126">Request body</span></span>
<span data-ttu-id="d29fd-127">В тексте запроса добавьте представление объекта [Виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d29fd-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="d29fd-128">В следующей таблице приведены свойства, необходимые при создании [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d29fd-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="d29fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d29fd-129">Property</span></span>|<span data-ttu-id="d29fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d29fd-130">Type</span></span>|<span data-ttu-id="d29fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d29fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d29fd-132">id</span><span class="sxs-lookup"><span data-stu-id="d29fd-132">id</span></span>|<span data-ttu-id="d29fd-133">String</span><span class="sxs-lookup"><span data-stu-id="d29fd-133">String</span></span>|<span data-ttu-id="d29fd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d29fd-134">Key of the entity.</span></span> <span data-ttu-id="d29fd-135">НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d29fd-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="d29fd-136">Модели</span><span class="sxs-lookup"><span data-stu-id="d29fd-136">appUserModelId</span></span>|<span data-ttu-id="d29fd-137">String</span><span class="sxs-lookup"><span data-stu-id="d29fd-137">String</span></span>|<span data-ttu-id="d29fd-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения приложения WindowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="d29fd-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="d29fd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d29fd-139">Response</span></span>
<span data-ttu-id="d29fd-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d29fd-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d29fd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d29fd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d29fd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d29fd-142">Request</span></span>
<span data-ttu-id="d29fd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d29fd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="d29fd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d29fd-144">Response</span></span>
<span data-ttu-id="d29fd-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d29fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





