---
title: Создание Микрософтсторефорбусинессконтаинедапп
description: Создание нового объекта Микрософтсторефорбусинессконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02e0617811683e13d72f8a014f458c42166f17ca
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172802"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="c6801-103">Создание Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="c6801-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="c6801-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6801-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6801-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6801-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6801-106">Создание нового объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c6801-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6801-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6801-107">Prerequisites</span></span>
<span data-ttu-id="c6801-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6801-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6801-110">Permission type</span></span>|<span data-ttu-id="c6801-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6801-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6801-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6801-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6801-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6801-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6801-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6801-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6801-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6801-115">Not supported.</span></span>|
|<span data-ttu-id="c6801-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6801-116">Application</span></span>|<span data-ttu-id="c6801-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6801-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6801-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6801-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="c6801-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6801-119">Request headers</span></span>
|<span data-ttu-id="c6801-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6801-120">Header</span></span>|<span data-ttu-id="c6801-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c6801-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6801-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6801-122">Authorization</span></span>|<span data-ttu-id="c6801-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6801-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6801-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c6801-124">Accept</span></span>|<span data-ttu-id="c6801-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6801-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6801-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6801-126">Request body</span></span>
<span data-ttu-id="c6801-127">В тексте запроса добавьте представление объекта Микрософтсторефорбусинессконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6801-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="c6801-128">В следующей таблице приведены свойства, необходимые при создании Микрософтсторефорбусинессконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="c6801-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="c6801-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6801-129">Property</span></span>|<span data-ttu-id="c6801-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c6801-130">Type</span></span>|<span data-ttu-id="c6801-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c6801-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6801-132">id</span><span class="sxs-lookup"><span data-stu-id="c6801-132">id</span></span>|<span data-ttu-id="c6801-133">String</span><span class="sxs-lookup"><span data-stu-id="c6801-133">String</span></span>|<span data-ttu-id="c6801-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c6801-134">Key of the entity.</span></span> <span data-ttu-id="c6801-135">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6801-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c6801-136">Модели</span><span class="sxs-lookup"><span data-stu-id="c6801-136">appUserModelId</span></span>|<span data-ttu-id="c6801-137">String.</span><span class="sxs-lookup"><span data-stu-id="c6801-137">String</span></span>|<span data-ttu-id="c6801-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="c6801-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="c6801-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6801-139">Response</span></span>
<span data-ttu-id="c6801-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6801-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6801-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c6801-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6801-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6801-142">Request</span></span>
<span data-ttu-id="c6801-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6801-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c6801-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6801-144">Response</span></span>
<span data-ttu-id="c6801-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6801-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```




