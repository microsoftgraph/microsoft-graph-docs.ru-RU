---
title: Обновление MicrosoftStoreForBusinessContainedApp
description: Обновление свойств объекта MicrosoftStoreForBusinessContainedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9062bb741bdb6c065129ab3b681cb4faed92e8e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139926"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="cda1f-103">Обновление MicrosoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="cda1f-103">Update microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="cda1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cda1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cda1f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cda1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda1f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cda1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda1f-107">Обновление свойств объекта [MicrosoftStoreForBusinessContainedApp.](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cda1f-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cda1f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cda1f-108">Prerequisites</span></span>
<span data-ttu-id="cda1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cda1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cda1f-111">Permission type</span></span>|<span data-ttu-id="cda1f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cda1f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda1f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cda1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cda1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cda1f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cda1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cda1f-116">Not supported.</span></span>|
|<span data-ttu-id="cda1f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cda1f-117">Application</span></span>|<span data-ttu-id="cda1f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda1f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cda1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cda1f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cda1f-120">Request headers</span></span>
|<span data-ttu-id="cda1f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cda1f-121">Header</span></span>|<span data-ttu-id="cda1f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cda1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cda1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda1f-123">Authorization</span></span>|<span data-ttu-id="cda1f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cda1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cda1f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cda1f-125">Accept</span></span>|<span data-ttu-id="cda1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cda1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda1f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cda1f-127">Request body</span></span>
<span data-ttu-id="cda1f-128">В теле запроса поставляем представление JSON для [объекта MicrosoftStoreForBusinessContainedApp.](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cda1f-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="cda1f-129">В следующей таблице показаны свойства, необходимые при создании [microsoftStoreForBusinessContainedApp.](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cda1f-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="cda1f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cda1f-130">Property</span></span>|<span data-ttu-id="cda1f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cda1f-131">Type</span></span>|<span data-ttu-id="cda1f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cda1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda1f-133">id</span><span class="sxs-lookup"><span data-stu-id="cda1f-133">id</span></span>|<span data-ttu-id="cda1f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cda1f-134">String</span></span>|<span data-ttu-id="cda1f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cda1f-135">Key of the entity.</span></span> <span data-ttu-id="cda1f-136">Унаследованный от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cda1f-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="cda1f-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="cda1f-137">appUserModelId</span></span>|<span data-ttu-id="cda1f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cda1f-138">String</span></span>|<span data-ttu-id="cda1f-139">ID модели пользователя приложения, содержатого приложения MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="cda1f-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="cda1f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda1f-140">Response</span></span>
<span data-ttu-id="cda1f-141">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cda1f-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda1f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="cda1f-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="cda1f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cda1f-143">Request</span></span>
<span data-ttu-id="cda1f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cda1f-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="cda1f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cda1f-145">Response</span></span>
<span data-ttu-id="cda1f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cda1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




