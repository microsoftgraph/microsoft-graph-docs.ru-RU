---
title: Действие assignedAccessMultiModeProfiles
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6304bd25dd0c54b3e90c98c637d4bc1976ab99a7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390644"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="88a24-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="88a24-103">assignedAccessMultiModeProfiles action</span></span>

<span data-ttu-id="88a24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88a24-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88a24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88a24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a24-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="88a24-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88a24-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="88a24-108">Prerequisites</span></span>
<span data-ttu-id="88a24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88a24-111">Permission type</span></span>|<span data-ttu-id="88a24-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88a24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88a24-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88a24-114">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="88a24-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a24-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a24-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="88a24-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88a24-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a24-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a24-117">Not supported.</span></span>|
|<span data-ttu-id="88a24-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88a24-118">Application</span></span>||
| <span data-ttu-id="88a24-119">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="88a24-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88a24-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88a24-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88a24-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88a24-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="88a24-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88a24-122">Request headers</span></span>
|<span data-ttu-id="88a24-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88a24-123">Header</span></span>|<span data-ttu-id="88a24-124">Значение</span><span class="sxs-lookup"><span data-stu-id="88a24-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a24-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88a24-125">Authorization</span></span>|<span data-ttu-id="88a24-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88a24-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a24-127">Accept</span><span class="sxs-lookup"><span data-stu-id="88a24-127">Accept</span></span>|<span data-ttu-id="88a24-128">application/json</span><span class="sxs-lookup"><span data-stu-id="88a24-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a24-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88a24-129">Request body</span></span>
<span data-ttu-id="88a24-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a24-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="88a24-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="88a24-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="88a24-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a24-132">Property</span></span>|<span data-ttu-id="88a24-133">Тип</span><span class="sxs-lookup"><span data-stu-id="88a24-133">Type</span></span>|<span data-ttu-id="88a24-134">Описание</span><span class="sxs-lookup"><span data-stu-id="88a24-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a24-135">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="88a24-135">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="88a24-136">Коллекция Виндовсассигнедакцесспрофиле</span><span class="sxs-lookup"><span data-stu-id="88a24-136">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="88a24-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="88a24-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="88a24-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="88a24-138">Response</span></span>
<span data-ttu-id="88a24-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88a24-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88a24-140">Пример</span><span class="sxs-lookup"><span data-stu-id="88a24-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a24-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="88a24-141">Request</span></span>
<span data-ttu-id="88a24-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88a24-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88a24-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a24-143">Response</span></span>
<span data-ttu-id="88a24-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88a24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






