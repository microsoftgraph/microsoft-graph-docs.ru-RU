---
title: Обновление Микрософтсторефорбусинессконтаинедапп
description: Обновление свойств объекта Микрософтсторефорбусинессконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ec387bdb0db79766cda0eb6a4dbc482c78bc50b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961114"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="bb1ac-103">Обновление Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="bb1ac-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="bb1ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb1ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb1ac-106">Обновление свойств объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bb1ac-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb1ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb1ac-107">Prerequisites</span></span>
<span data-ttu-id="bb1ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb1ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb1ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb1ac-110">Permission type</span></span>|<span data-ttu-id="bb1ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb1ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb1ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb1ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb1ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb1ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb1ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb1ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb1ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-115">Not supported.</span></span>|
|<span data-ttu-id="bb1ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb1ac-116">Application</span></span>|<span data-ttu-id="bb1ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb1ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb1ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bb1ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb1ac-119">Request headers</span></span>
|<span data-ttu-id="bb1ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb1ac-120">Header</span></span>|<span data-ttu-id="bb1ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bb1ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb1ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb1ac-122">Authorization</span></span>|<span data-ttu-id="bb1ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb1ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb1ac-124">Accept</span></span>|<span data-ttu-id="bb1ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb1ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb1ac-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb1ac-126">Request body</span></span>
<span data-ttu-id="bb1ac-127">В тексте запроса добавьте представление объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="bb1ac-128">В следующей таблице приведены свойства, необходимые при создании [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb1ac-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="bb1ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb1ac-129">Property</span></span>|<span data-ttu-id="bb1ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb1ac-130">Type</span></span>|<span data-ttu-id="bb1ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb1ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb1ac-132">id</span><span class="sxs-lookup"><span data-stu-id="bb1ac-132">id</span></span>|<span data-ttu-id="bb1ac-133">String</span><span class="sxs-lookup"><span data-stu-id="bb1ac-133">String</span></span>|<span data-ttu-id="bb1ac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-134">Key of the entity.</span></span> <span data-ttu-id="bb1ac-135">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb1ac-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="bb1ac-136">Модели</span><span class="sxs-lookup"><span data-stu-id="bb1ac-136">appUserModelId</span></span>|<span data-ttu-id="bb1ac-137">String</span><span class="sxs-lookup"><span data-stu-id="bb1ac-137">String</span></span>|<span data-ttu-id="bb1ac-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="bb1ac-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb1ac-139">Response</span></span>
<span data-ttu-id="bb1ac-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb1ac-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bb1ac-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb1ac-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb1ac-142">Request</span></span>
<span data-ttu-id="bb1ac-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="bb1ac-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb1ac-144">Response</span></span>
<span data-ttu-id="bb1ac-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb1ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





