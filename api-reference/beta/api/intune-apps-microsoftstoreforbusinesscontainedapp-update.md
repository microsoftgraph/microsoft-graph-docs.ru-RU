---
title: Обновление microsoftStoreForBusinessContainedApp
description: Обновление свойства объекта microsoftStoreForBusinessContainedApp.
ms.openlocfilehash: b5a946a79b5040778cce24deaee3326f93380e76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082464"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="954c8-103">Обновление microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="954c8-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="954c8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="954c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="954c8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="954c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="954c8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="954c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="954c8-107">Обновление свойства объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="954c8-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="954c8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="954c8-108">Prerequisites</span></span>
<span data-ttu-id="954c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="954c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="954c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="954c8-111">Permission type</span></span>|<span data-ttu-id="954c8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="954c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="954c8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="954c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="954c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="954c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="954c8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="954c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="954c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="954c8-116">Not supported.</span></span>|
|<span data-ttu-id="954c8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="954c8-117">Application</span></span>|<span data-ttu-id="954c8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="954c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="954c8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="954c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="954c8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="954c8-120">Request headers</span></span>
|<span data-ttu-id="954c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="954c8-121">Header</span></span>|<span data-ttu-id="954c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="954c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="954c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="954c8-123">Authorization</span></span>|<span data-ttu-id="954c8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="954c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="954c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="954c8-125">Accept</span></span>|<span data-ttu-id="954c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="954c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="954c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="954c8-127">Request body</span></span>
<span data-ttu-id="954c8-128">В тексте запроса укажите представление JSON для объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="954c8-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="954c8-129">В следующей таблице показаны свойства, которые необходимы для создания [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="954c8-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="954c8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="954c8-130">Property</span></span>|<span data-ttu-id="954c8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="954c8-131">Type</span></span>|<span data-ttu-id="954c8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="954c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="954c8-133">id</span><span class="sxs-lookup"><span data-stu-id="954c8-133">id</span></span>|<span data-ttu-id="954c8-134">String</span><span class="sxs-lookup"><span data-stu-id="954c8-134">String</span></span>|<span data-ttu-id="954c8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="954c8-135">Key of the entity.</span></span> <span data-ttu-id="954c8-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="954c8-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="954c8-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="954c8-137">appUserModelId</span></span>|<span data-ttu-id="954c8-138">String</span><span class="sxs-lookup"><span data-stu-id="954c8-138">String</span></span>|<span data-ttu-id="954c8-139">Автономные приложения MicrosoftStoreForBusinessApp модели пользователя приложения.</span><span class="sxs-lookup"><span data-stu-id="954c8-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="954c8-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="954c8-140">Response</span></span>
<span data-ttu-id="954c8-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="954c8-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="954c8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="954c8-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="954c8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="954c8-143">Request</span></span>
<span data-ttu-id="954c8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="954c8-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="954c8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="954c8-145">Response</span></span>
<span data-ttu-id="954c8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="954c8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





