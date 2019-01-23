---
title: Обновление windowsUniversalAppXContainedApp
description: Обновление свойства объекта windowsUniversalAppXContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b396d7d1c2995f9e65db63622ad421a481cfe9de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405613"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="8d131-103">Обновление windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="8d131-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="8d131-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d131-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d131-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d131-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d131-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d131-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d131-107">Обновление свойства объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8d131-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d131-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8d131-108">Prerequisites</span></span>
<span data-ttu-id="8d131-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d131-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d131-111">Permission type</span></span>|<span data-ttu-id="8d131-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d131-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d131-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d131-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d131-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d131-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d131-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d131-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d131-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d131-116">Not supported.</span></span>|
|<span data-ttu-id="8d131-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d131-117">Application</span></span>|<span data-ttu-id="8d131-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d131-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d131-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d131-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8d131-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d131-120">Request headers</span></span>
|<span data-ttu-id="8d131-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d131-121">Header</span></span>|<span data-ttu-id="8d131-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d131-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d131-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d131-123">Authorization</span></span>|<span data-ttu-id="8d131-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d131-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d131-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d131-125">Accept</span></span>|<span data-ttu-id="8d131-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d131-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d131-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d131-127">Request body</span></span>
<span data-ttu-id="8d131-128">В тексте запроса укажите представление JSON для объекта [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8d131-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="8d131-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d131-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="8d131-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d131-130">Property</span></span>|<span data-ttu-id="8d131-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d131-131">Type</span></span>|<span data-ttu-id="8d131-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d131-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d131-133">id</span><span class="sxs-lookup"><span data-stu-id="8d131-133">id</span></span>|<span data-ttu-id="8d131-134">String</span><span class="sxs-lookup"><span data-stu-id="8d131-134">String</span></span>|<span data-ttu-id="8d131-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d131-135">Key of the entity.</span></span> <span data-ttu-id="8d131-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d131-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="8d131-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="8d131-137">appUserModelId</span></span>|<span data-ttu-id="8d131-138">String</span><span class="sxs-lookup"><span data-stu-id="8d131-138">String</span></span>|<span data-ttu-id="8d131-139">Идентификатор модели пользователя приложения автономные приложения WindowsUniversalAppX приложения.</span><span class="sxs-lookup"><span data-stu-id="8d131-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="8d131-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d131-140">Response</span></span>
<span data-ttu-id="8d131-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d131-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d131-142">Пример</span><span class="sxs-lookup"><span data-stu-id="8d131-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d131-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d131-143">Request</span></span>
<span data-ttu-id="8d131-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d131-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="8d131-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d131-145">Response</span></span>
<span data-ttu-id="8d131-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d131-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




