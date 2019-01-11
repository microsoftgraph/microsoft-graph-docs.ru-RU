---
title: Обновление windowsUniversalAppXContainedApp
description: Обновление свойства объекта windowsUniversalAppXContainedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 642921c66bfbc996c5c3b0f3f16cf812c75a5618
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882343"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="ea120-103">Обновление windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="ea120-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="ea120-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea120-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea120-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea120-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea120-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea120-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea120-107">Обновление свойства объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ea120-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea120-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea120-108">Prerequisites</span></span>
<span data-ttu-id="ea120-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea120-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea120-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea120-111">Permission type</span></span>|<span data-ttu-id="ea120-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea120-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea120-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea120-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea120-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea120-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea120-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea120-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea120-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea120-116">Not supported.</span></span>|
|<span data-ttu-id="ea120-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea120-117">Application</span></span>|<span data-ttu-id="ea120-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea120-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea120-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea120-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ea120-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea120-120">Request headers</span></span>
|<span data-ttu-id="ea120-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea120-121">Header</span></span>|<span data-ttu-id="ea120-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea120-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea120-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea120-123">Authorization</span></span>|<span data-ttu-id="ea120-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ea120-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea120-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea120-125">Accept</span></span>|<span data-ttu-id="ea120-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea120-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea120-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea120-127">Request body</span></span>
<span data-ttu-id="ea120-128">В тексте запроса укажите представление JSON для объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ea120-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="ea120-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ea120-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="ea120-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea120-130">Property</span></span>|<span data-ttu-id="ea120-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea120-131">Type</span></span>|<span data-ttu-id="ea120-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea120-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea120-133">id</span><span class="sxs-lookup"><span data-stu-id="ea120-133">id</span></span>|<span data-ttu-id="ea120-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ea120-134">String</span></span>|<span data-ttu-id="ea120-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea120-135">Key of the entity.</span></span> <span data-ttu-id="ea120-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea120-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="ea120-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="ea120-137">appUserModelId</span></span>|<span data-ttu-id="ea120-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ea120-138">String</span></span>|<span data-ttu-id="ea120-139">Идентификатор модели пользователя приложения автономные приложения WindowsUniversalAppX приложения.</span><span class="sxs-lookup"><span data-stu-id="ea120-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="ea120-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea120-140">Response</span></span>
<span data-ttu-id="ea120-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea120-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea120-142">Пример</span><span class="sxs-lookup"><span data-stu-id="ea120-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea120-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea120-143">Request</span></span>
<span data-ttu-id="ea120-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea120-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="ea120-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea120-145">Response</span></span>
<span data-ttu-id="ea120-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea120-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





