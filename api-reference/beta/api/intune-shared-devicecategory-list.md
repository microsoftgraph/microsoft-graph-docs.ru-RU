---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e20c9f31c5174dfc60d8d589bae1a5f51de8972a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898467"
---
# <a name="list-devicecategories"></a><span data-ttu-id="e5549-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="e5549-103">List deviceCategories</span></span>

> <span data-ttu-id="e5549-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5549-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5549-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5549-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5549-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5549-107">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e5549-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5549-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e5549-108">Prerequisites</span></span>
<span data-ttu-id="e5549-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5549-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5549-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5549-111">Permission type</span></span>|<span data-ttu-id="e5549-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5549-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5549-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5549-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e5549-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="e5549-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e5549-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5549-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e5549-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5549-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5549-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5549-117">Not supported.</span></span>|
|<span data-ttu-id="e5549-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5549-118">Application</span></span>|<span data-ttu-id="e5549-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5549-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5549-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5549-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="e5549-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5549-121">Request headers</span></span>

|<span data-ttu-id="e5549-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5549-122">Header</span></span>|<span data-ttu-id="e5549-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e5549-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5549-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5549-124">Authorization</span></span>|<span data-ttu-id="e5549-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5549-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5549-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e5549-126">Accept</span></span>|<span data-ttu-id="e5549-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5549-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5549-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5549-128">Request body</span></span>

<span data-ttu-id="e5549-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5549-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5549-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5549-130">Response</span></span>

<span data-ttu-id="e5549-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5549-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5549-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e5549-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5549-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5549-133">Request</span></span>

<span data-ttu-id="e5549-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5549-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="e5549-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5549-135">Response</span></span>

<span data-ttu-id="e5549-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5549-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



