---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7b4286d967274eafeafa3797d2fa57633f52e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458884"
---
# <a name="list-devicecategories"></a><span data-ttu-id="7d8f4-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7d8f4-103">List deviceCategories</span></span>

<span data-ttu-id="7d8f4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d8f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d8f4-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d8f4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d8f4-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d8f4-108">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7d8f4-108">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d8f4-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d8f4-109">Prerequisites</span></span>
<span data-ttu-id="7d8f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d8f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d8f4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d8f4-112">Permission type</span></span>|<span data-ttu-id="7d8f4-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d8f4-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d8f4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d8f4-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7d8f4-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7d8f4-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7d8f4-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d8f4-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7d8f4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d8f4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d8f4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-118">Not supported.</span></span>|
|<span data-ttu-id="7d8f4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d8f4-119">Application</span></span>||
| <span data-ttu-id="7d8f4-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7d8f4-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7d8f4-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d8f4-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d8f4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d8f4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="7d8f4-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d8f4-123">Request headers</span></span>

|<span data-ttu-id="7d8f4-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d8f4-124">Header</span></span>|<span data-ttu-id="7d8f4-125">Значение</span><span class="sxs-lookup"><span data-stu-id="7d8f4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d8f4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8f4-126">Authorization</span></span>|<span data-ttu-id="7d8f4-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d8f4-128">Accept</span><span class="sxs-lookup"><span data-stu-id="7d8f4-128">Accept</span></span>|<span data-ttu-id="7d8f4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7d8f4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8f4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d8f4-130">Request body</span></span>

<span data-ttu-id="7d8f4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d8f4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d8f4-132">Response</span></span>

<span data-ttu-id="7d8f4-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-133">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8f4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7d8f4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d8f4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d8f4-135">Request</span></span>

<span data-ttu-id="7d8f4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="7d8f4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d8f4-137">Response</span></span>

<span data-ttu-id="7d8f4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d8f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











