---
title: Действие assignedAccessMultiModeProfiles
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55528d2676976dff7466b9f949dbe5ca03f2d8a1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537059"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="2c85c-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="2c85c-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="2c85c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c85c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c85c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c85c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c85c-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2c85c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c85c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2c85c-107">Prerequisites</span></span>
<span data-ttu-id="2c85c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c85c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c85c-110">Permission type</span></span>|<span data-ttu-id="2c85c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c85c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c85c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c85c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2c85c-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="2c85c-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2c85c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c85c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2c85c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c85c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c85c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c85c-116">Not supported.</span></span>|
|<span data-ttu-id="2c85c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2c85c-117">Application</span></span>||
| <span data-ttu-id="2c85c-118">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="2c85c-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2c85c-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c85c-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c85c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c85c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2c85c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c85c-121">Request headers</span></span>
|<span data-ttu-id="2c85c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c85c-122">Header</span></span>|<span data-ttu-id="2c85c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2c85c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c85c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c85c-124">Authorization</span></span>|<span data-ttu-id="2c85c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c85c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c85c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2c85c-126">Accept</span></span>|<span data-ttu-id="2c85c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c85c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c85c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c85c-128">Request body</span></span>
<span data-ttu-id="2c85c-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c85c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2c85c-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2c85c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2c85c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c85c-131">Property</span></span>|<span data-ttu-id="2c85c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2c85c-132">Type</span></span>|<span data-ttu-id="2c85c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2c85c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c85c-134">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="2c85c-134">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="2c85c-135">Коллекция Виндовсассигнедакцесспрофиле</span><span class="sxs-lookup"><span data-stu-id="2c85c-135">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="2c85c-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2c85c-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2c85c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c85c-137">Response</span></span>
<span data-ttu-id="2c85c-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c85c-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c85c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2c85c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c85c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c85c-140">Request</span></span>
<span data-ttu-id="2c85c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c85c-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2c85c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c85c-142">Response</span></span>
<span data-ttu-id="2c85c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c85c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






