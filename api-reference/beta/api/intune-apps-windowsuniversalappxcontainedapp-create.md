---
title: Создание windowsUniversalAppXContainedApp
description: Создание нового объекта windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0466628ed1b2e6f3e0e196498b7cef3bb9daf24
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920984"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="86d36-103">Создание windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="86d36-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="86d36-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86d36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86d36-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86d36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86d36-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="86d36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86d36-107">Создание нового объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="86d36-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86d36-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86d36-108">Prerequisites</span></span>
<span data-ttu-id="86d36-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86d36-111">Permission type</span></span>|<span data-ttu-id="86d36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86d36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86d36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86d36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86d36-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d36-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86d36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86d36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86d36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86d36-116">Not supported.</span></span>|
|<span data-ttu-id="86d36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86d36-117">Application</span></span>|<span data-ttu-id="86d36-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86d36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86d36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86d36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="86d36-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86d36-120">Request headers</span></span>
|<span data-ttu-id="86d36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86d36-121">Header</span></span>|<span data-ttu-id="86d36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86d36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d36-123">Authorization</span></span>|<span data-ttu-id="86d36-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="86d36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86d36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86d36-125">Accept</span></span>|<span data-ttu-id="86d36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86d36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86d36-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86d36-127">Request body</span></span>
<span data-ttu-id="86d36-128">В тексте запроса укажите представление JSON для объекта windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="86d36-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="86d36-129">В следующей таблице показаны свойства, которые необходимы для создания windowsUniversalAppXContainedApp.</span><span class="sxs-lookup"><span data-stu-id="86d36-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="86d36-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86d36-130">Property</span></span>|<span data-ttu-id="86d36-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86d36-131">Type</span></span>|<span data-ttu-id="86d36-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86d36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86d36-133">id</span><span class="sxs-lookup"><span data-stu-id="86d36-133">id</span></span>|<span data-ttu-id="86d36-134">String</span><span class="sxs-lookup"><span data-stu-id="86d36-134">String</span></span>|<span data-ttu-id="86d36-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86d36-135">Key of the entity.</span></span> <span data-ttu-id="86d36-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="86d36-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="86d36-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="86d36-137">appUserModelId</span></span>|<span data-ttu-id="86d36-138">String</span><span class="sxs-lookup"><span data-stu-id="86d36-138">String</span></span>|<span data-ttu-id="86d36-139">Идентификатор модели пользователя приложения автономные приложения WindowsUniversalAppX приложения.</span><span class="sxs-lookup"><span data-stu-id="86d36-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="86d36-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="86d36-140">Response</span></span>
<span data-ttu-id="86d36-141">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86d36-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86d36-142">Пример</span><span class="sxs-lookup"><span data-stu-id="86d36-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="86d36-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="86d36-143">Request</span></span>
<span data-ttu-id="86d36-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86d36-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="86d36-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="86d36-145">Response</span></span>
<span data-ttu-id="86d36-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="86d36-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





