---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92afadc514c036211cba932b6e7f2b8f3a76ace7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201132"
---
# <a name="assign-action"></a><span data-ttu-id="fdeab-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="fdeab-103">assign action</span></span>

> <span data-ttu-id="fdeab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdeab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdeab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdeab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdeab-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fdeab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdeab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fdeab-107">Prerequisites</span></span>
<span data-ttu-id="fdeab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdeab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdeab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdeab-110">Permission type</span></span>|<span data-ttu-id="fdeab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdeab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdeab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdeab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdeab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdeab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdeab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdeab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdeab-115">Not supported.</span></span>|
|<span data-ttu-id="fdeab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdeab-116">Application</span></span>|<span data-ttu-id="fdeab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdeab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdeab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fdeab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdeab-119">Request headers</span></span>
|<span data-ttu-id="fdeab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdeab-120">Header</span></span>|<span data-ttu-id="fdeab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fdeab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdeab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdeab-122">Authorization</span></span>|<span data-ttu-id="fdeab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdeab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdeab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fdeab-124">Accept</span></span>|<span data-ttu-id="fdeab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fdeab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdeab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdeab-126">Request body</span></span>
<span data-ttu-id="fdeab-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdeab-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fdeab-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fdeab-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fdeab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdeab-129">Property</span></span>|<span data-ttu-id="fdeab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fdeab-130">Type</span></span>|<span data-ttu-id="fdeab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fdeab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdeab-132">assignments</span><span class="sxs-lookup"><span data-stu-id="fdeab-132">assignments</span></span>|<span data-ttu-id="fdeab-133">Коллекция [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fdeab-133">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="fdeab-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fdeab-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fdeab-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdeab-135">Response</span></span>
<span data-ttu-id="fdeab-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fdeab-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdeab-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fdeab-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdeab-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdeab-138">Request</span></span>
<span data-ttu-id="fdeab-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdeab-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assign

Content-type: application/json
Content-length: 285

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
      "id": "567a744f-744f-567a-4f74-7a564f747a56",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fdeab-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdeab-140">Response</span></span>
<span data-ttu-id="fdeab-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdeab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




