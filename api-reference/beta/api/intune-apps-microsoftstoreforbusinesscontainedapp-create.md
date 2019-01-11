---
title: Создание microsoftStoreForBusinessContainedApp
description: Создание нового объекта microsoftStoreForBusinessContainedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac782261c00008bf9b4ab552932f8f841a9965bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843297"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="1be86-103">Создание microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="1be86-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="1be86-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1be86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1be86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1be86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1be86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1be86-107">Создание нового объекта [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="1be86-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1be86-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1be86-108">Prerequisites</span></span>
<span data-ttu-id="1be86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1be86-111">Permission type</span></span>|<span data-ttu-id="1be86-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1be86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1be86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1be86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1be86-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be86-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1be86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1be86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1be86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be86-116">Not supported.</span></span>|
|<span data-ttu-id="1be86-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1be86-117">Application</span></span>|<span data-ttu-id="1be86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1be86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1be86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="1be86-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1be86-120">Request headers</span></span>
|<span data-ttu-id="1be86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1be86-121">Header</span></span>|<span data-ttu-id="1be86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1be86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1be86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be86-123">Authorization</span></span>|<span data-ttu-id="1be86-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1be86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1be86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1be86-125">Accept</span></span>|<span data-ttu-id="1be86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1be86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1be86-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1be86-127">Request body</span></span>
<span data-ttu-id="1be86-128">В тексте запроса укажите представление JSON для объекта microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="1be86-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="1be86-129">В следующей таблице показаны свойства, которые необходимы для создания microsoftStoreForBusinessContainedApp.</span><span class="sxs-lookup"><span data-stu-id="1be86-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="1be86-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1be86-130">Property</span></span>|<span data-ttu-id="1be86-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1be86-131">Type</span></span>|<span data-ttu-id="1be86-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1be86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be86-133">id</span><span class="sxs-lookup"><span data-stu-id="1be86-133">id</span></span>|<span data-ttu-id="1be86-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1be86-134">String</span></span>|<span data-ttu-id="1be86-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1be86-135">Key of the entity.</span></span> <span data-ttu-id="1be86-136">Наследуется от [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1be86-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="1be86-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="1be86-137">appUserModelId</span></span>|<span data-ttu-id="1be86-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1be86-138">String</span></span>|<span data-ttu-id="1be86-139">Автономные приложения MicrosoftStoreForBusinessApp модели пользователя приложения.</span><span class="sxs-lookup"><span data-stu-id="1be86-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="1be86-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be86-140">Response</span></span>
<span data-ttu-id="1be86-141">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1be86-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1be86-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1be86-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="1be86-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be86-143">Request</span></span>
<span data-ttu-id="1be86-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1be86-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="1be86-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be86-145">Response</span></span>
<span data-ttu-id="1be86-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1be86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





