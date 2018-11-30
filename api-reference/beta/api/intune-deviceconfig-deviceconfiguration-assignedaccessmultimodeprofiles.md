---
title: Действие assignedAccessMultiModeProfiles
description: Н/Д
ms.openlocfilehash: eb4e4cce71baabfcd10d28b88438dd2e4fe989c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078463"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="9354c-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="9354c-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="9354c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9354c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9354c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9354c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9354c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9354c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9354c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9354c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9354c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9354c-108">Prerequisites</span></span>
<span data-ttu-id="9354c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9354c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9354c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9354c-111">Permission type</span></span>|<span data-ttu-id="9354c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9354c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9354c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9354c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9354c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9354c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9354c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9354c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9354c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9354c-116">Not supported.</span></span>|
|<span data-ttu-id="9354c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9354c-117">Application</span></span>|<span data-ttu-id="9354c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9354c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9354c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9354c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9354c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9354c-120">Request headers</span></span>
|<span data-ttu-id="9354c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9354c-121">Header</span></span>|<span data-ttu-id="9354c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9354c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9354c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9354c-123">Authorization</span></span>|<span data-ttu-id="9354c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9354c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9354c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9354c-125">Accept</span></span>|<span data-ttu-id="9354c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9354c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9354c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9354c-127">Request body</span></span>
<span data-ttu-id="9354c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9354c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9354c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9354c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9354c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9354c-130">Property</span></span>|<span data-ttu-id="9354c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9354c-131">Type</span></span>|<span data-ttu-id="9354c-132">Description</span><span class="sxs-lookup"><span data-stu-id="9354c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9354c-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="9354c-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="9354c-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9354c-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="9354c-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9354c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9354c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9354c-136">Response</span></span>
<span data-ttu-id="9354c-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9354c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9354c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9354c-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9354c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9354c-139">Request</span></span>
<span data-ttu-id="9354c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9354c-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9354c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="9354c-141">Response</span></span>
<span data-ttu-id="9354c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9354c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





