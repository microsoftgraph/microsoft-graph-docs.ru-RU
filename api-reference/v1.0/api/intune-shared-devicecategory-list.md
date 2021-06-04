---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65d69d7602c66a18edc0f4cf50d52a39aeefd2a0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732722"
---
# <a name="list-devicecategories"></a><span data-ttu-id="3a40e-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3a40e-103">List deviceCategories</span></span>

<span data-ttu-id="3a40e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a40e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a40e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a40e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a40e-106">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="3a40e-106">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a40e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3a40e-107">Prerequisites</span></span>
<span data-ttu-id="3a40e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a40e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a40e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a40e-110">Permission type</span></span>|<span data-ttu-id="3a40e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a40e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a40e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a40e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3a40e-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="3a40e-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3a40e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a40e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3a40e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a40e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a40e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a40e-116">Not supported.</span></span>|
|<span data-ttu-id="3a40e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a40e-117">Application</span></span>|<span data-ttu-id="3a40e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a40e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a40e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a40e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="3a40e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a40e-120">Request headers</span></span>
|<span data-ttu-id="3a40e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a40e-121">Header</span></span>|<span data-ttu-id="3a40e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a40e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a40e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a40e-123">Authorization</span></span>|<span data-ttu-id="3a40e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a40e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a40e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a40e-125">Accept</span></span>|<span data-ttu-id="3a40e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a40e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a40e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a40e-127">Request body</span></span>
<span data-ttu-id="3a40e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a40e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a40e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a40e-129">Response</span></span>
<span data-ttu-id="3a40e-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a40e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a40e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a40e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a40e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a40e-132">Request</span></span>
<span data-ttu-id="3a40e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a40e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="3a40e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a40e-134">Response</span></span>
<span data-ttu-id="3a40e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a40e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









