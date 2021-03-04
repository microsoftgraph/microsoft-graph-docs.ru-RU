---
title: Список deviceManagementConfigurationCategories
description: Список свойств и связей объектов deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3282f9e3d98865cc01e99fe2a171b1dfc36e9136
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441587"
---
# <a name="list-devicemanagementconfigurationcategories"></a><span data-ttu-id="160b8-103">Список deviceManagementConfigurationCategories</span><span class="sxs-lookup"><span data-stu-id="160b8-103">List deviceManagementConfigurationCategories</span></span>

<span data-ttu-id="160b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="160b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="160b8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="160b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="160b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="160b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="160b8-107">Список свойств и связей [объектов deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="160b8-107">List properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="160b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="160b8-108">Prerequisites</span></span>
<span data-ttu-id="160b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="160b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="160b8-111">Permission type</span></span>|<span data-ttu-id="160b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="160b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="160b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="160b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="160b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="160b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="160b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="160b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="160b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="160b8-116">Not supported.</span></span>|
|<span data-ttu-id="160b8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="160b8-117">Application</span></span>|<span data-ttu-id="160b8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="160b8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="160b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="160b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="160b8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="160b8-120">Request headers</span></span>
|<span data-ttu-id="160b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="160b8-121">Header</span></span>|<span data-ttu-id="160b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="160b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="160b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="160b8-123">Authorization</span></span>|<span data-ttu-id="160b8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="160b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="160b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="160b8-125">Accept</span></span>|<span data-ttu-id="160b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="160b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="160b8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="160b8-127">Request body</span></span>
<span data-ttu-id="160b8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="160b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="160b8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="160b8-129">Response</span></span>
<span data-ttu-id="160b8-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="160b8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160b8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="160b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="160b8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="160b8-132">Request</span></span>
<span data-ttu-id="160b8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="160b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationCategories
```

### <a name="response"></a><span data-ttu-id="160b8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="160b8-134">Response</span></span>
<span data-ttu-id="160b8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="160b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 603

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
      "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "platforms": "macOS",
      "technologies": "mdm",
      "settingUsage": "configuration",
      "parentCategoryId": "Parent Category Id value",
      "rootCategoryId": "Root Category Id value",
      "childCategoryIds": [
        "Child Category Ids value"
      ]
    }
  ]
}
```




