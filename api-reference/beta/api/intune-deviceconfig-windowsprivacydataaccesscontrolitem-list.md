---
title: Список Виндовспривацидатаакцессконтролитемс
description: Список свойств и связей объектов Виндовспривацидатаакцессконтролитем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1941618fad1258e5b88f4dea2c47c06400b09884
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732568"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="95aeb-103">Список Виндовспривацидатаакцессконтролитемс</span><span class="sxs-lookup"><span data-stu-id="95aeb-103">List windowsPrivacyDataAccessControlItems</span></span>

> <span data-ttu-id="95aeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95aeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95aeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95aeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95aeb-106">Список свойств и связей объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="95aeb-106">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95aeb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95aeb-107">Prerequisites</span></span>
<span data-ttu-id="95aeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95aeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95aeb-110">Permission type</span></span>|<span data-ttu-id="95aeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95aeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95aeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95aeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95aeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95aeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95aeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95aeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95aeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95aeb-115">Not supported.</span></span>|
|<span data-ttu-id="95aeb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="95aeb-116">Application</span></span>|<span data-ttu-id="95aeb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95aeb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95aeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95aeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="95aeb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95aeb-119">Request headers</span></span>
|<span data-ttu-id="95aeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95aeb-120">Header</span></span>|<span data-ttu-id="95aeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95aeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95aeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95aeb-122">Authorization</span></span>|<span data-ttu-id="95aeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95aeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95aeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95aeb-124">Accept</span></span>|<span data-ttu-id="95aeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95aeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95aeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95aeb-126">Request body</span></span>
<span data-ttu-id="95aeb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95aeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95aeb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="95aeb-128">Response</span></span>
<span data-ttu-id="95aeb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95aeb-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95aeb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95aeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95aeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95aeb-131">Request</span></span>
<span data-ttu-id="95aeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95aeb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="95aeb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="95aeb-133">Response</span></span>
<span data-ttu-id="95aeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95aeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
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




