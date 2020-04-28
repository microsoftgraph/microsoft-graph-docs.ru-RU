---
title: Создание Микрософтсторефорбусинессконтаинедапп
description: Создание нового объекта Микрософтсторефорбусинессконтаинедапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f068fc347ebc0352ccaf9e627cc3cfb35f57721
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404921"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="b6760-103">Создание Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="b6760-103">Create microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="b6760-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6760-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6760-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6760-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6760-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6760-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6760-107">Создание нового объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b6760-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6760-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6760-108">Prerequisites</span></span>
<span data-ttu-id="b6760-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6760-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6760-111">Permission type</span></span>|<span data-ttu-id="b6760-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6760-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6760-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6760-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6760-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6760-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6760-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6760-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6760-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6760-116">Not supported.</span></span>|
|<span data-ttu-id="b6760-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6760-117">Application</span></span>|<span data-ttu-id="b6760-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6760-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6760-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6760-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="b6760-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6760-120">Request headers</span></span>
|<span data-ttu-id="b6760-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6760-121">Header</span></span>|<span data-ttu-id="b6760-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6760-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6760-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6760-123">Authorization</span></span>|<span data-ttu-id="b6760-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6760-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6760-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6760-125">Accept</span></span>|<span data-ttu-id="b6760-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6760-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6760-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6760-127">Request body</span></span>
<span data-ttu-id="b6760-128">В тексте запроса добавьте представление объекта Микрософтсторефорбусинессконтаинедапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6760-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="b6760-129">В следующей таблице приведены свойства, необходимые при создании Микрософтсторефорбусинессконтаинедапп.</span><span class="sxs-lookup"><span data-stu-id="b6760-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="b6760-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6760-130">Property</span></span>|<span data-ttu-id="b6760-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6760-131">Type</span></span>|<span data-ttu-id="b6760-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b6760-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6760-133">id</span><span class="sxs-lookup"><span data-stu-id="b6760-133">id</span></span>|<span data-ttu-id="b6760-134">String</span><span class="sxs-lookup"><span data-stu-id="b6760-134">String</span></span>|<span data-ttu-id="b6760-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6760-135">Key of the entity.</span></span> <span data-ttu-id="b6760-136">Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6760-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="b6760-137">Модели</span><span class="sxs-lookup"><span data-stu-id="b6760-137">appUserModelId</span></span>|<span data-ttu-id="b6760-138">String</span><span class="sxs-lookup"><span data-stu-id="b6760-138">String</span></span>|<span data-ttu-id="b6760-139">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="b6760-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="b6760-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6760-140">Response</span></span>
<span data-ttu-id="b6760-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6760-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6760-142">Пример</span><span class="sxs-lookup"><span data-stu-id="b6760-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6760-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6760-143">Request</span></span>
<span data-ttu-id="b6760-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6760-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="b6760-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6760-145">Response</span></span>
<span data-ttu-id="b6760-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6760-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



