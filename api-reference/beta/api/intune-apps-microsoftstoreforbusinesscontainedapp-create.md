---
title: Создание microsoftStoreForBusinessContainedApp
description: Создание нового объекта microsoftStoreForBusinessContainedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1286ccdd3f87f7669b13c63063c0bc78e8cc633
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421139"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="f3c0d-103">Создание microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="f3c0d-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="f3c0d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3c0d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3c0d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c0d-107">Создание нового объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f3c0d-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3c0d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f3c0d-108">Prerequisites</span></span>
<span data-ttu-id="f3c0d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3c0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3c0d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c0d-111">Permission type</span></span>|<span data-ttu-id="f3c0d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3c0d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3c0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3c0d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3c0d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-116">Not supported.</span></span>|
|<span data-ttu-id="f3c0d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c0d-117">Application</span></span>|<span data-ttu-id="f3c0d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3c0d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="f3c0d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c0d-120">Request headers</span></span>
|<span data-ttu-id="f3c0d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c0d-121">Header</span></span>|<span data-ttu-id="f3c0d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3c0d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c0d-123">Authorization</span></span>|<span data-ttu-id="f3c0d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f3c0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3c0d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3c0d-125">Accept</span></span>|<span data-ttu-id="f3c0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3c0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3c0d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3c0d-127">Request body</span></span>
<span data-ttu-id="f3c0d-128">В тексте запроса укажите представление JSON для объекта microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="f3c0d-129">В следующей таблице показаны свойства, которые необходимы для создания microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="f3c0d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3c0d-130">Property</span></span>|<span data-ttu-id="f3c0d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3c0d-131">Type</span></span>|<span data-ttu-id="f3c0d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3c0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c0d-133">id</span><span class="sxs-lookup"><span data-stu-id="f3c0d-133">id</span></span>|<span data-ttu-id="f3c0d-134">String</span><span class="sxs-lookup"><span data-stu-id="f3c0d-134">String</span></span>|<span data-ttu-id="f3c0d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-135">Key of the entity.</span></span> <span data-ttu-id="f3c0d-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3c0d-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="f3c0d-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="f3c0d-137">appUserModelId</span></span>|<span data-ttu-id="f3c0d-138">String</span><span class="sxs-lookup"><span data-stu-id="f3c0d-138">String</span></span>|<span data-ttu-id="f3c0d-139">Автономные приложения MicrosoftStoreForBusinessApp модели пользователя приложения.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="f3c0d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c0d-140">Response</span></span>
<span data-ttu-id="f3c0d-141">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3c0d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c0d-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3c0d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c0d-143">Request</span></span>
<span data-ttu-id="f3c0d-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f3c0d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c0d-145">Response</span></span>
<span data-ttu-id="f3c0d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f3c0d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




