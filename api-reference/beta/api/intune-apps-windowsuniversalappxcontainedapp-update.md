---
title: Обновление windowsUniversalAppXContainedApp
description: Обновление свойства объекта windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a00075adac27b22b0e533fa922eb9077c88344d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941032"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="dd161-103">Обновление windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="dd161-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="dd161-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd161-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd161-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd161-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd161-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd161-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd161-107">Обновление свойства объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="dd161-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd161-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd161-108">Prerequisites</span></span>
<span data-ttu-id="dd161-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd161-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd161-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd161-111">Permission type</span></span>|<span data-ttu-id="dd161-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd161-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd161-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd161-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd161-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd161-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd161-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd161-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd161-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd161-116">Not supported.</span></span>|
|<span data-ttu-id="dd161-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd161-117">Application</span></span>|<span data-ttu-id="dd161-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd161-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd161-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd161-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="dd161-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd161-120">Request headers</span></span>
|<span data-ttu-id="dd161-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd161-121">Header</span></span>|<span data-ttu-id="dd161-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd161-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd161-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd161-123">Authorization</span></span>|<span data-ttu-id="dd161-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dd161-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd161-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd161-125">Accept</span></span>|<span data-ttu-id="dd161-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd161-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd161-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd161-127">Request body</span></span>
<span data-ttu-id="dd161-128">В тексте запроса укажите представление JSON для объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="dd161-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="dd161-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd161-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="dd161-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd161-130">Property</span></span>|<span data-ttu-id="dd161-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd161-131">Type</span></span>|<span data-ttu-id="dd161-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd161-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd161-133">id</span><span class="sxs-lookup"><span data-stu-id="dd161-133">id</span></span>|<span data-ttu-id="dd161-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dd161-134">String</span></span>|<span data-ttu-id="dd161-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd161-135">Key of the entity.</span></span> <span data-ttu-id="dd161-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd161-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="dd161-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="dd161-137">appUserModelId</span></span>|<span data-ttu-id="dd161-138">Строка</span><span class="sxs-lookup"><span data-stu-id="dd161-138">String</span></span>|<span data-ttu-id="dd161-139">Идентификатор модели пользователя приложения автономные приложения WindowsUniversalAppX приложения.</span><span class="sxs-lookup"><span data-stu-id="dd161-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="dd161-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd161-140">Response</span></span>
<span data-ttu-id="dd161-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dd161-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd161-142">Пример</span><span class="sxs-lookup"><span data-stu-id="dd161-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd161-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd161-143">Request</span></span>
<span data-ttu-id="dd161-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd161-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="dd161-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd161-145">Response</span></span>
<span data-ttu-id="dd161-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dd161-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





