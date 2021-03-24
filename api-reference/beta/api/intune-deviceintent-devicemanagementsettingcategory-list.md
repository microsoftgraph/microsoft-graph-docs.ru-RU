---
title: Список deviceManagementSettingCategories
description: Список свойств и связей объектов deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62c0185fc4a196f2d3895e2166f7db4ab5cae21f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136666"
---
# <a name="list-devicemanagementsettingcategories"></a><span data-ttu-id="f4bbc-103">Список deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="f4bbc-103">List deviceManagementSettingCategories</span></span>

<span data-ttu-id="f4bbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4bbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4bbc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4bbc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4bbc-107">Список свойств и связей [объектов deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f4bbc-107">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4bbc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4bbc-108">Prerequisites</span></span>
<span data-ttu-id="f4bbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4bbc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4bbc-111">Permission type</span></span>|<span data-ttu-id="f4bbc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4bbc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4bbc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4bbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4bbc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4bbc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4bbc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4bbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4bbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-116">Not supported.</span></span>|
|<span data-ttu-id="f4bbc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4bbc-117">Application</span></span>|<span data-ttu-id="f4bbc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4bbc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4bbc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4bbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/categories
```

## <a name="request-headers"></a><span data-ttu-id="f4bbc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4bbc-120">Request headers</span></span>
|<span data-ttu-id="f4bbc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4bbc-121">Header</span></span>|<span data-ttu-id="f4bbc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4bbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4bbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4bbc-123">Authorization</span></span>|<span data-ttu-id="f4bbc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4bbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4bbc-125">Accept</span></span>|<span data-ttu-id="f4bbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4bbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4bbc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4bbc-127">Request body</span></span>
<span data-ttu-id="f4bbc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4bbc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4bbc-129">Response</span></span>
<span data-ttu-id="f4bbc-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4bbc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4bbc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4bbc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4bbc-132">Request</span></span>
<span data-ttu-id="f4bbc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/categories
```

### <a name="response"></a><span data-ttu-id="f4bbc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4bbc-134">Response</span></span>
<span data-ttu-id="f4bbc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4bbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
      "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
      "displayName": "Display Name value",
      "hasRequiredSetting": true
    }
  ]
}
```




