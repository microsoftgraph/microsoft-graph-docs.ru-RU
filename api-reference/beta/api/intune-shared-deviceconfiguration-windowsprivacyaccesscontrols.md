---
title: Действие windowsPrivacyAccessControls
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5826c36fdc749de1851ec53439828da49c39daad
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801203"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="c2841-103">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="c2841-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="c2841-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2841-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2841-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2841-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2841-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c2841-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2841-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2841-107">Prerequisites</span></span>
<span data-ttu-id="c2841-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2841-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2841-110">Permission type</span></span>|<span data-ttu-id="c2841-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2841-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2841-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2841-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c2841-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c2841-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c2841-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2841-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2841-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2841-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2841-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2841-116">Not supported.</span></span>|
|<span data-ttu-id="c2841-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2841-117">Application</span></span>||
| <span data-ttu-id="c2841-118">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c2841-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c2841-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2841-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2841-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2841-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="c2841-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2841-121">Request headers</span></span>
|<span data-ttu-id="c2841-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2841-122">Header</span></span>|<span data-ttu-id="c2841-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c2841-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2841-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2841-124">Authorization</span></span>|<span data-ttu-id="c2841-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2841-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2841-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c2841-126">Accept</span></span>|<span data-ttu-id="c2841-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c2841-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2841-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2841-128">Request body</span></span>
<span data-ttu-id="c2841-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2841-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c2841-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c2841-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c2841-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2841-131">Property</span></span>|<span data-ttu-id="c2841-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c2841-132">Type</span></span>|<span data-ttu-id="c2841-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c2841-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2841-134">виндовспривациакцессконтролс</span><span class="sxs-lookup"><span data-stu-id="c2841-134">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="c2841-135">Коллекция [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2841-135">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="c2841-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c2841-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c2841-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2841-137">Response</span></span>
<span data-ttu-id="c2841-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2841-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2841-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c2841-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2841-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2841-140">Request</span></span>
<span data-ttu-id="c2841-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2841-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 379

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c2841-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2841-142">Response</span></span>
<span data-ttu-id="c2841-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2841-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







