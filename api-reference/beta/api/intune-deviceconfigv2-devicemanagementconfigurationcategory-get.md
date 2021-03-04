---
title: Get deviceManagementConfigurationCategory
description: Чтение свойств и связей объекта deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7b76ca23b5a89d2f8d33ebcbfd39ff3948012e6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441601"
---
# <a name="get-devicemanagementconfigurationcategory"></a><span data-ttu-id="17499-103">Get deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="17499-103">Get deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="17499-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17499-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17499-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17499-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17499-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17499-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17499-107">Чтение свойств и связей [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="17499-107">Read properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17499-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17499-108">Prerequisites</span></span>
<span data-ttu-id="17499-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17499-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17499-111">Permission type</span></span>|<span data-ttu-id="17499-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17499-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17499-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17499-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17499-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17499-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17499-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17499-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17499-116">Not supported.</span></span>|
|<span data-ttu-id="17499-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17499-117">Application</span></span>|<span data-ttu-id="17499-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17499-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17499-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17499-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17499-120">Optional query parameters</span></span>
<span data-ttu-id="17499-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17499-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17499-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17499-122">Request headers</span></span>
|<span data-ttu-id="17499-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17499-123">Header</span></span>|<span data-ttu-id="17499-124">Значение</span><span class="sxs-lookup"><span data-stu-id="17499-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17499-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17499-125">Authorization</span></span>|<span data-ttu-id="17499-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17499-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17499-127">Accept</span><span class="sxs-lookup"><span data-stu-id="17499-127">Accept</span></span>|<span data-ttu-id="17499-128">application/json</span><span class="sxs-lookup"><span data-stu-id="17499-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17499-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17499-129">Request body</span></span>
<span data-ttu-id="17499-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17499-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17499-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="17499-131">Response</span></span>
<span data-ttu-id="17499-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17499-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17499-133">Пример</span><span class="sxs-lookup"><span data-stu-id="17499-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="17499-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="17499-134">Request</span></span>
<span data-ttu-id="17499-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17499-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

### <a name="response"></a><span data-ttu-id="17499-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="17499-136">Response</span></span>
<span data-ttu-id="17499-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17499-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "value": {
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
}
```




