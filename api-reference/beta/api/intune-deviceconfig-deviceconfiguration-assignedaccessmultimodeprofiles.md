---
title: Действие assignedAccessMultiModeProfiles
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 094276c28cad82d60958e97d65134672f333c579
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346025"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="f6a9a-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="f6a9a-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="f6a9a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6a9a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6a9a-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6a9a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6a9a-107">Prerequisites</span></span>
<span data-ttu-id="f6a9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6a9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6a9a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6a9a-110">Permission type</span></span>|<span data-ttu-id="f6a9a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6a9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6a9a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6a9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6a9a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6a9a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6a9a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6a9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6a9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-115">Not supported.</span></span>|
|<span data-ttu-id="f6a9a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6a9a-116">Application</span></span>|<span data-ttu-id="f6a9a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6a9a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6a9a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6a9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f6a9a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6a9a-119">Request headers</span></span>
|<span data-ttu-id="f6a9a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6a9a-120">Header</span></span>|<span data-ttu-id="f6a9a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6a9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6a9a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6a9a-122">Authorization</span></span>|<span data-ttu-id="f6a9a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6a9a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f6a9a-124">Accept</span></span>|<span data-ttu-id="f6a9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6a9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6a9a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6a9a-126">Request body</span></span>
<span data-ttu-id="f6a9a-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f6a9a-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f6a9a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6a9a-129">Property</span></span>|<span data-ttu-id="f6a9a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a9a-130">Type</span></span>|<span data-ttu-id="f6a9a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6a9a-132">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="f6a9a-132">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="f6a9a-133">Коллекция Виндовсассигнедакцесспрофиле</span><span class="sxs-lookup"><span data-stu-id="f6a9a-133">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="f6a9a-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f6a9a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6a9a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6a9a-135">Response</span></span>
<span data-ttu-id="f6a9a-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6a9a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f6a9a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6a9a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6a9a-138">Request</span></span>
<span data-ttu-id="f6a9a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6a9a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6a9a-140">Response</span></span>
<span data-ttu-id="f6a9a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6a9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






