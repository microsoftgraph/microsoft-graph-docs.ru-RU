---
title: Обновление microsoftStoreForBusinessContainedApp
description: Обновление свойства объекта microsoftStoreForBusinessContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a1154555af19db7d56778d454cdc07ce647f324
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417198"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="dbe37-103">Обновление microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="dbe37-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="dbe37-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbe37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dbe37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbe37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbe37-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbe37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe37-107">Обновление свойства объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="dbe37-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbe37-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="dbe37-108">Prerequisites</span></span>
<span data-ttu-id="dbe37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dbe37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dbe37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbe37-111">Permission type</span></span>|<span data-ttu-id="dbe37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbe37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbe37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbe37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbe37-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe37-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbe37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbe37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbe37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbe37-116">Not supported.</span></span>|
|<span data-ttu-id="dbe37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbe37-117">Application</span></span>|<span data-ttu-id="dbe37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbe37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbe37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbe37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="dbe37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbe37-120">Request headers</span></span>
|<span data-ttu-id="dbe37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbe37-121">Header</span></span>|<span data-ttu-id="dbe37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dbe37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbe37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe37-123">Authorization</span></span>|<span data-ttu-id="dbe37-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dbe37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbe37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dbe37-125">Accept</span></span>|<span data-ttu-id="dbe37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbe37-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbe37-127">Request body</span></span>
<span data-ttu-id="dbe37-128">В тексте запроса укажите представление JSON для объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="dbe37-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="dbe37-129">В следующей таблице показаны свойства, которые необходимы для создания [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dbe37-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="dbe37-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbe37-130">Property</span></span>|<span data-ttu-id="dbe37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dbe37-131">Type</span></span>|<span data-ttu-id="dbe37-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dbe37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe37-133">id</span><span class="sxs-lookup"><span data-stu-id="dbe37-133">id</span></span>|<span data-ttu-id="dbe37-134">String</span><span class="sxs-lookup"><span data-stu-id="dbe37-134">String</span></span>|<span data-ttu-id="dbe37-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dbe37-135">Key of the entity.</span></span> <span data-ttu-id="dbe37-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbe37-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="dbe37-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="dbe37-137">appUserModelId</span></span>|<span data-ttu-id="dbe37-138">String</span><span class="sxs-lookup"><span data-stu-id="dbe37-138">String</span></span>|<span data-ttu-id="dbe37-139">Автономные приложения MicrosoftStoreForBusinessApp модели пользователя приложения.</span><span class="sxs-lookup"><span data-stu-id="dbe37-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="dbe37-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbe37-140">Response</span></span>
<span data-ttu-id="dbe37-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dbe37-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe37-142">Пример</span><span class="sxs-lookup"><span data-stu-id="dbe37-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbe37-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbe37-143">Request</span></span>
<span data-ttu-id="dbe37-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbe37-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="dbe37-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbe37-145">Response</span></span>
<span data-ttu-id="dbe37-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dbe37-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```




