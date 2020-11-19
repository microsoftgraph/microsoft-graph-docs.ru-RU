---
title: Действие assignedAccessMultiModeProfiles
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed16d86975783eea6a85fdf2e67febc830b0b03d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232546"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="76fb0-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="76fb0-103">assignedAccessMultiModeProfiles action</span></span>

<span data-ttu-id="76fb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76fb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76fb0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76fb0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76fb0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76fb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76fb0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="76fb0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76fb0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76fb0-108">Prerequisites</span></span>
<span data-ttu-id="76fb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76fb0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76fb0-111">Permission type</span></span>|<span data-ttu-id="76fb0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76fb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76fb0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76fb0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="76fb0-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="76fb0-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="76fb0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76fb0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="76fb0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76fb0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76fb0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76fb0-117">Not supported.</span></span>|
|<span data-ttu-id="76fb0-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="76fb0-118">Application</span></span>||
| <span data-ttu-id="76fb0-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="76fb0-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="76fb0-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76fb0-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76fb0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76fb0-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="76fb0-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76fb0-122">Request headers</span></span>
|<span data-ttu-id="76fb0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76fb0-123">Header</span></span>|<span data-ttu-id="76fb0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="76fb0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76fb0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76fb0-125">Authorization</span></span>|<span data-ttu-id="76fb0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76fb0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76fb0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="76fb0-127">Accept</span></span>|<span data-ttu-id="76fb0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="76fb0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76fb0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76fb0-129">Request body</span></span>
<span data-ttu-id="76fb0-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76fb0-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="76fb0-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="76fb0-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="76fb0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="76fb0-132">Property</span></span>|<span data-ttu-id="76fb0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="76fb0-133">Type</span></span>|<span data-ttu-id="76fb0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="76fb0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76fb0-135">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="76fb0-135">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="76fb0-136">Коллекция Виндовсассигнедакцесспрофиле</span><span class="sxs-lookup"><span data-stu-id="76fb0-136">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="76fb0-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="76fb0-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="76fb0-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="76fb0-138">Response</span></span>
<span data-ttu-id="76fb0-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76fb0-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76fb0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="76fb0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="76fb0-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="76fb0-141">Request</span></span>
<span data-ttu-id="76fb0-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76fb0-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76fb0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="76fb0-143">Response</span></span>
<span data-ttu-id="76fb0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76fb0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







