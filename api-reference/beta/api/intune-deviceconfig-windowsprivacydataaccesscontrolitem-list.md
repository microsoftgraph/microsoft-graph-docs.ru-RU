---
title: Список Виндовспривацидатаакцессконтролитемс
description: Список свойств и связей объектов Виндовспривацидатаакцессконтролитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 738b00aec531e9153f56d295fbc2de6785947905
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730968"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="f7bbf-103">Список Виндовспривацидатаакцессконтролитемс</span><span class="sxs-lookup"><span data-stu-id="f7bbf-103">List windowsPrivacyDataAccessControlItems</span></span>

<span data-ttu-id="f7bbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7bbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7bbf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7bbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7bbf-107">Список свойств и связей объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f7bbf-107">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7bbf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7bbf-108">Prerequisites</span></span>
<span data-ttu-id="f7bbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7bbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7bbf-111">Permission type</span></span>|<span data-ttu-id="f7bbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7bbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7bbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7bbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7bbf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7bbf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f7bbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7bbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-116">Not supported.</span></span>|
|<span data-ttu-id="f7bbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7bbf-117">Application</span></span>|<span data-ttu-id="f7bbf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7bbf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7bbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7bbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="f7bbf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7bbf-120">Request headers</span></span>
|<span data-ttu-id="f7bbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7bbf-121">Header</span></span>|<span data-ttu-id="f7bbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7bbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7bbf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7bbf-123">Authorization</span></span>|<span data-ttu-id="f7bbf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7bbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7bbf-125">Accept</span></span>|<span data-ttu-id="f7bbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7bbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7bbf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7bbf-127">Request body</span></span>
<span data-ttu-id="f7bbf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7bbf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7bbf-129">Response</span></span>
<span data-ttu-id="f7bbf-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7bbf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f7bbf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7bbf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7bbf-132">Request</span></span>
<span data-ttu-id="f7bbf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="f7bbf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7bbf-134">Response</span></span>
<span data-ttu-id="f7bbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7bbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





