---
title: Список Виндовспривацидатаакцессконтролитемс
description: Список свойств и связей объектов Виндовспривацидатаакцессконтролитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13954efbd0104b52f0fd2fe8c77ef91d342e2ae7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473880"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="ecf2e-103">Список Виндовспривацидатаакцессконтролитемс</span><span class="sxs-lookup"><span data-stu-id="ecf2e-103">List windowsPrivacyDataAccessControlItems</span></span>

<span data-ttu-id="ecf2e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ecf2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecf2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecf2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecf2e-107">Список свойств и связей объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ecf2e-107">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecf2e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ecf2e-108">Prerequisites</span></span>
<span data-ttu-id="ecf2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecf2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecf2e-111">Permission type</span></span>|<span data-ttu-id="ecf2e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecf2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecf2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecf2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecf2e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecf2e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ecf2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecf2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecf2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-116">Not supported.</span></span>|
|<span data-ttu-id="ecf2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecf2e-117">Application</span></span>|<span data-ttu-id="ecf2e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecf2e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecf2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecf2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="ecf2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ecf2e-120">Request headers</span></span>
|<span data-ttu-id="ecf2e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecf2e-121">Header</span></span>|<span data-ttu-id="ecf2e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ecf2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecf2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecf2e-123">Authorization</span></span>|<span data-ttu-id="ecf2e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecf2e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecf2e-125">Accept</span></span>|<span data-ttu-id="ecf2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecf2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecf2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecf2e-127">Request body</span></span>
<span data-ttu-id="ecf2e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecf2e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecf2e-129">Response</span></span>
<span data-ttu-id="ecf2e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf2e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ecf2e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecf2e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecf2e-132">Request</span></span>
<span data-ttu-id="ecf2e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="ecf2e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecf2e-134">Response</span></span>
<span data-ttu-id="ecf2e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecf2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





