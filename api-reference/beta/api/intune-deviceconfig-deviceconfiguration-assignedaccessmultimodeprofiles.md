---
title: Действие assignedAccessMultiModeProfiles
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e52d3ee24223f56b0047b87f0d526329fd99ff79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944427"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="8e249-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="8e249-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="8e249-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e249-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e249-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e249-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e249-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e249-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e249-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8e249-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e249-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8e249-108">Prerequisites</span></span>
<span data-ttu-id="8e249-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e249-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e249-111">Permission type</span></span>|<span data-ttu-id="8e249-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e249-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e249-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e249-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e249-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e249-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8e249-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e249-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e249-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e249-116">Not supported.</span></span>|
|<span data-ttu-id="8e249-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e249-117">Application</span></span>|<span data-ttu-id="8e249-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e249-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e249-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e249-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8e249-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e249-120">Request headers</span></span>
|<span data-ttu-id="8e249-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e249-121">Header</span></span>|<span data-ttu-id="8e249-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e249-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e249-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e249-123">Authorization</span></span>|<span data-ttu-id="8e249-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e249-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e249-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e249-125">Accept</span></span>|<span data-ttu-id="8e249-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e249-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e249-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e249-127">Request body</span></span>
<span data-ttu-id="8e249-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e249-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8e249-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8e249-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8e249-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e249-130">Property</span></span>|<span data-ttu-id="8e249-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e249-131">Type</span></span>|<span data-ttu-id="8e249-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e249-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e249-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="8e249-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="8e249-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8e249-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="8e249-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8e249-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8e249-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e249-136">Response</span></span>
<span data-ttu-id="8e249-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e249-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e249-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8e249-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e249-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e249-139">Request</span></span>
<span data-ttu-id="8e249-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e249-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e249-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e249-141">Response</span></span>
<span data-ttu-id="8e249-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8e249-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





