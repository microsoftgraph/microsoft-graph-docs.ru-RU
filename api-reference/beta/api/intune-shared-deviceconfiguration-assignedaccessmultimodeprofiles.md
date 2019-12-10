---
title: Действие assignedAccessMultiModeProfiles
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9795d48fe744b78e301933d15aef48237e0e4343
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940084"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="09cde-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="09cde-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="09cde-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09cde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09cde-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09cde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09cde-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="09cde-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09cde-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09cde-107">Prerequisites</span></span>
<span data-ttu-id="09cde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09cde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09cde-110">Permission type</span></span>|<span data-ttu-id="09cde-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09cde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09cde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09cde-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="09cde-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="09cde-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09cde-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09cde-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09cde-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09cde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09cde-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09cde-116">Not supported.</span></span>|
|<span data-ttu-id="09cde-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09cde-117">Application</span></span>||
| <span data-ttu-id="09cde-118">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="09cde-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09cde-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09cde-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09cde-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09cde-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="09cde-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09cde-121">Request headers</span></span>
|<span data-ttu-id="09cde-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09cde-122">Header</span></span>|<span data-ttu-id="09cde-123">Значение</span><span class="sxs-lookup"><span data-stu-id="09cde-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09cde-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09cde-124">Authorization</span></span>|<span data-ttu-id="09cde-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09cde-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09cde-126">Accept</span><span class="sxs-lookup"><span data-stu-id="09cde-126">Accept</span></span>|<span data-ttu-id="09cde-127">application/json</span><span class="sxs-lookup"><span data-stu-id="09cde-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09cde-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09cde-128">Request body</span></span>
<span data-ttu-id="09cde-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09cde-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="09cde-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="09cde-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="09cde-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="09cde-131">Property</span></span>|<span data-ttu-id="09cde-132">Тип</span><span class="sxs-lookup"><span data-stu-id="09cde-132">Type</span></span>|<span data-ttu-id="09cde-133">Описание</span><span class="sxs-lookup"><span data-stu-id="09cde-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09cde-134">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="09cde-134">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="09cde-135">Коллекция Виндовсассигнедакцесспрофиле</span><span class="sxs-lookup"><span data-stu-id="09cde-135">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="09cde-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="09cde-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="09cde-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="09cde-137">Response</span></span>
<span data-ttu-id="09cde-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09cde-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09cde-139">Пример</span><span class="sxs-lookup"><span data-stu-id="09cde-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="09cde-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="09cde-140">Request</span></span>
<span data-ttu-id="09cde-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09cde-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09cde-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="09cde-142">Response</span></span>
<span data-ttu-id="09cde-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09cde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








