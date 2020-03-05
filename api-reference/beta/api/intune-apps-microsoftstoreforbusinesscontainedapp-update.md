---
title: Обновление Микрософтсторефорбусинессконтаинедапп
description: Обновление свойств объекта Микрософтсторефорбусинессконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a25ce46c353902feb700bdf1a853d3998f34eee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450848"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="f0453-103">Обновление Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="f0453-103">Update microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="f0453-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0453-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0453-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0453-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0453-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0453-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0453-107">Обновление свойств объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f0453-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0453-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0453-108">Prerequisites</span></span>
<span data-ttu-id="f0453-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0453-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0453-111">Permission type</span></span>|<span data-ttu-id="f0453-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0453-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0453-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0453-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0453-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0453-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0453-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0453-116">Not supported.</span></span>|
|<span data-ttu-id="f0453-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0453-117">Application</span></span>|<span data-ttu-id="f0453-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0453-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0453-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f0453-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0453-120">Request headers</span></span>
|<span data-ttu-id="f0453-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0453-121">Header</span></span>|<span data-ttu-id="f0453-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0453-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0453-123">Authorization</span></span>|<span data-ttu-id="f0453-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0453-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0453-125">Accept</span></span>|<span data-ttu-id="f0453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0453-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0453-127">Request body</span></span>
<span data-ttu-id="f0453-128">В тексте запроса добавьте представление объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0453-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="f0453-129">В следующей таблице приведены свойства, необходимые при создании [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0453-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="f0453-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0453-130">Property</span></span>|<span data-ttu-id="f0453-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0453-131">Type</span></span>|<span data-ttu-id="f0453-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0453-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0453-133">id</span><span class="sxs-lookup"><span data-stu-id="f0453-133">id</span></span>|<span data-ttu-id="f0453-134">String</span><span class="sxs-lookup"><span data-stu-id="f0453-134">String</span></span>|<span data-ttu-id="f0453-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0453-135">Key of the entity.</span></span> <span data-ttu-id="f0453-136">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0453-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="f0453-137">Модели</span><span class="sxs-lookup"><span data-stu-id="f0453-137">appUserModelId</span></span>|<span data-ttu-id="f0453-138">String</span><span class="sxs-lookup"><span data-stu-id="f0453-138">String</span></span>|<span data-ttu-id="f0453-139">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="f0453-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="f0453-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0453-140">Response</span></span>
<span data-ttu-id="f0453-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0453-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0453-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f0453-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0453-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0453-143">Request</span></span>
<span data-ttu-id="f0453-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0453-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f0453-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0453-145">Response</span></span>
<span data-ttu-id="f0453-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0453-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





