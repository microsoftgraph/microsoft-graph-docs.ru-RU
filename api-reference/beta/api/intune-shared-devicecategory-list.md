---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2eb8250715686fc427bfe82510eb984aa683235
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980381"
---
# <a name="list-devicecategories"></a><span data-ttu-id="abaae-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="abaae-103">List deviceCategories</span></span>

<span data-ttu-id="abaae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abaae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abaae-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abaae-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="abaae-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abaae-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abaae-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abaae-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abaae-108">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="abaae-108">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abaae-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="abaae-109">Prerequisites</span></span>
<span data-ttu-id="abaae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abaae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abaae-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abaae-112">Permission type</span></span>|<span data-ttu-id="abaae-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abaae-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abaae-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abaae-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="abaae-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="abaae-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="abaae-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="abaae-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="abaae-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abaae-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abaae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abaae-118">Not supported.</span></span>|
|<span data-ttu-id="abaae-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abaae-119">Application</span></span>||
| <span data-ttu-id="abaae-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="abaae-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="abaae-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="abaae-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abaae-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abaae-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="abaae-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="abaae-123">Request headers</span></span>

|<span data-ttu-id="abaae-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abaae-124">Header</span></span>|<span data-ttu-id="abaae-125">Значение</span><span class="sxs-lookup"><span data-stu-id="abaae-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abaae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="abaae-126">Authorization</span></span>|<span data-ttu-id="abaae-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abaae-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abaae-128">Accept</span><span class="sxs-lookup"><span data-stu-id="abaae-128">Accept</span></span>|<span data-ttu-id="abaae-129">application/json</span><span class="sxs-lookup"><span data-stu-id="abaae-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abaae-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abaae-130">Request body</span></span>

<span data-ttu-id="abaae-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abaae-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abaae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="abaae-132">Response</span></span>

<span data-ttu-id="abaae-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="abaae-133">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abaae-134">Пример</span><span class="sxs-lookup"><span data-stu-id="abaae-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="abaae-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="abaae-135">Request</span></span>

<span data-ttu-id="abaae-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abaae-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="abaae-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="abaae-137">Response</span></span>

<span data-ttu-id="abaae-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abaae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```












