---
title: Список windowsPrivacyDataAccessControlItems
description: Список свойств и связей объектов windowsPrivacyDataAccesssControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 752213b89b4d1da3cfbfbc97b53961aaa6c50254
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154660"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="803ae-103">Список windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="803ae-103">List windowsPrivacyDataAccessControlItems</span></span>

<span data-ttu-id="803ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="803ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="803ae-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="803ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="803ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="803ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="803ae-107">Список свойств и связей [объектов windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="803ae-107">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="803ae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="803ae-108">Prerequisites</span></span>
<span data-ttu-id="803ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="803ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="803ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="803ae-111">Permission type</span></span>|<span data-ttu-id="803ae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="803ae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="803ae-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="803ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="803ae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="803ae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="803ae-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="803ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="803ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="803ae-116">Not supported.</span></span>|
|<span data-ttu-id="803ae-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="803ae-117">Application</span></span>|<span data-ttu-id="803ae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="803ae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="803ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="803ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="803ae-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="803ae-120">Request headers</span></span>
|<span data-ttu-id="803ae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="803ae-121">Header</span></span>|<span data-ttu-id="803ae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="803ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="803ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="803ae-123">Authorization</span></span>|<span data-ttu-id="803ae-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="803ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="803ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="803ae-125">Accept</span></span>|<span data-ttu-id="803ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="803ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="803ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="803ae-127">Request body</span></span>
<span data-ttu-id="803ae-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="803ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="803ae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="803ae-129">Response</span></span>
<span data-ttu-id="803ae-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="803ae-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="803ae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="803ae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="803ae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="803ae-132">Request</span></span>
<span data-ttu-id="803ae-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="803ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="803ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="803ae-134">Response</span></span>
<span data-ttu-id="803ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="803ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




