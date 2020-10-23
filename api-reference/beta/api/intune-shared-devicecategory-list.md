---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ca3429de3f7179e4bfa0e6dea5adb82b32af611
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729021"
---
# <a name="list-devicecategories"></a><span data-ttu-id="56221-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="56221-103">List deviceCategories</span></span>

<span data-ttu-id="56221-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56221-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56221-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56221-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56221-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56221-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56221-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56221-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56221-108">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="56221-108">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56221-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="56221-109">Prerequisites</span></span>
<span data-ttu-id="56221-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56221-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56221-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56221-112">Permission type</span></span>|<span data-ttu-id="56221-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56221-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56221-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56221-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="56221-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="56221-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="56221-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="56221-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="56221-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56221-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56221-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56221-118">Not supported.</span></span>|
|<span data-ttu-id="56221-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56221-119">Application</span></span>||
| <span data-ttu-id="56221-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="56221-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="56221-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="56221-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56221-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56221-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="56221-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="56221-123">Request headers</span></span>

|<span data-ttu-id="56221-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56221-124">Header</span></span>|<span data-ttu-id="56221-125">Значение</span><span class="sxs-lookup"><span data-stu-id="56221-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56221-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56221-126">Authorization</span></span>|<span data-ttu-id="56221-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56221-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56221-128">Accept</span><span class="sxs-lookup"><span data-stu-id="56221-128">Accept</span></span>|<span data-ttu-id="56221-129">application/json</span><span class="sxs-lookup"><span data-stu-id="56221-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56221-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56221-130">Request body</span></span>

<span data-ttu-id="56221-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56221-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56221-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="56221-132">Response</span></span>

<span data-ttu-id="56221-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="56221-133">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56221-134">Пример</span><span class="sxs-lookup"><span data-stu-id="56221-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="56221-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="56221-135">Request</span></span>

<span data-ttu-id="56221-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56221-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="56221-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="56221-137">Response</span></span>

<span data-ttu-id="56221-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56221-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











