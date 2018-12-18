---
title: Действие assignedAccessMultiModeProfiles
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 24ab12236044c08ab17b50acb5d7cc486fadcafa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358144"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="aa8bc-103">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="aa8bc-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="aa8bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa8bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa8bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa8bc-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa8bc-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa8bc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aa8bc-108">Prerequisites</span></span>
<span data-ttu-id="aa8bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa8bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa8bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa8bc-111">Permission type</span></span>|<span data-ttu-id="aa8bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa8bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa8bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa8bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa8bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa8bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aa8bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa8bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa8bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-116">Not supported.</span></span>|
|<span data-ttu-id="aa8bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa8bc-117">Application</span></span>|<span data-ttu-id="aa8bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa8bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa8bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="aa8bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa8bc-120">Request headers</span></span>
|<span data-ttu-id="aa8bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa8bc-121">Header</span></span>|<span data-ttu-id="aa8bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa8bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa8bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa8bc-123">Authorization</span></span>|<span data-ttu-id="aa8bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aa8bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa8bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa8bc-125">Accept</span></span>|<span data-ttu-id="aa8bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa8bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa8bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa8bc-127">Request body</span></span>
<span data-ttu-id="aa8bc-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aa8bc-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa8bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa8bc-130">Property</span></span>|<span data-ttu-id="aa8bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aa8bc-131">Type</span></span>|<span data-ttu-id="aa8bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aa8bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8bc-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="aa8bc-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="aa8bc-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="aa8bc-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="aa8bc-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa8bc-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aa8bc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa8bc-136">Response</span></span>
<span data-ttu-id="aa8bc-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa8bc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="aa8bc-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa8bc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa8bc-139">Request</span></span>
<span data-ttu-id="aa8bc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa8bc-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa8bc-141">Response</span></span>
<span data-ttu-id="aa8bc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aa8bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





