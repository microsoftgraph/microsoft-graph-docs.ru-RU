---
title: Обновление Микрософтсторефорбусинессконтаинедапп
description: Обновление свойств объекта Микрософтсторефорбусинессконтаинедапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20526c67ba34a2e508b625f8bc2fafeb9ba0b2eb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798595"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="efbd8-103">Обновление Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="efbd8-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="efbd8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efbd8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efbd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbd8-106">Обновление свойств объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="efbd8-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efbd8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efbd8-107">Prerequisites</span></span>
<span data-ttu-id="efbd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efbd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efbd8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efbd8-110">Permission type</span></span>|<span data-ttu-id="efbd8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efbd8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efbd8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efbd8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efbd8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbd8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efbd8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efbd8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efbd8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbd8-115">Not supported.</span></span>|
|<span data-ttu-id="efbd8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efbd8-116">Application</span></span>|<span data-ttu-id="efbd8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbd8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efbd8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efbd8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="efbd8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efbd8-119">Request headers</span></span>
|<span data-ttu-id="efbd8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efbd8-120">Header</span></span>|<span data-ttu-id="efbd8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="efbd8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efbd8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efbd8-122">Authorization</span></span>|<span data-ttu-id="efbd8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efbd8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efbd8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="efbd8-124">Accept</span></span>|<span data-ttu-id="efbd8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efbd8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efbd8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efbd8-126">Request body</span></span>
<span data-ttu-id="efbd8-127">В тексте запроса добавьте представление объекта [Микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efbd8-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="efbd8-128">В следующей таблице приведены свойства, необходимые при создании [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="efbd8-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="efbd8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="efbd8-129">Property</span></span>|<span data-ttu-id="efbd8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="efbd8-130">Type</span></span>|<span data-ttu-id="efbd8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="efbd8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efbd8-132">id</span><span class="sxs-lookup"><span data-stu-id="efbd8-132">id</span></span>|<span data-ttu-id="efbd8-133">String</span><span class="sxs-lookup"><span data-stu-id="efbd8-133">String</span></span>|<span data-ttu-id="efbd8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="efbd8-134">Key of the entity.</span></span> <span data-ttu-id="efbd8-135">НаСледуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="efbd8-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="efbd8-136">Модели</span><span class="sxs-lookup"><span data-stu-id="efbd8-136">appUserModelId</span></span>|<span data-ttu-id="efbd8-137">String</span><span class="sxs-lookup"><span data-stu-id="efbd8-137">String</span></span>|<span data-ttu-id="efbd8-138">ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="efbd8-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="efbd8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="efbd8-139">Response</span></span>
<span data-ttu-id="efbd8-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efbd8-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efbd8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="efbd8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="efbd8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="efbd8-142">Request</span></span>
<span data-ttu-id="efbd8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efbd8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="efbd8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="efbd8-144">Response</span></span>
<span data-ttu-id="efbd8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efbd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





