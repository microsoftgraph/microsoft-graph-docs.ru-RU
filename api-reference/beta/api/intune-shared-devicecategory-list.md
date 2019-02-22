---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40f138305b9f148bb48c4d4398024a8766a2bd5f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169323"
---
# <a name="list-devicecategories"></a><span data-ttu-id="0aca3-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0aca3-103">List deviceCategories</span></span>

> <span data-ttu-id="0aca3-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0aca3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0aca3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aca3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0aca3-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0aca3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aca3-107">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0aca3-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0aca3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0aca3-108">Prerequisites</span></span>
<span data-ttu-id="0aca3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aca3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="0aca3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0aca3-111">Permission type</span></span>|<span data-ttu-id="0aca3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0aca3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aca3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0aca3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0aca3-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="0aca3-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0aca3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aca3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0aca3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0aca3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aca3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aca3-117">Not supported.</span></span>|
|<span data-ttu-id="0aca3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0aca3-118">Application</span></span>|<span data-ttu-id="0aca3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aca3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aca3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0aca3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="0aca3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0aca3-121">Request headers</span></span>

|<span data-ttu-id="0aca3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0aca3-122">Header</span></span>|<span data-ttu-id="0aca3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0aca3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aca3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0aca3-124">Authorization</span></span>|<span data-ttu-id="0aca3-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0aca3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aca3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0aca3-126">Accept</span></span>|<span data-ttu-id="0aca3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0aca3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aca3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0aca3-128">Request body</span></span>

<span data-ttu-id="0aca3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0aca3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aca3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aca3-130">Response</span></span>

<span data-ttu-id="0aca3-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0aca3-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aca3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0aca3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aca3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0aca3-133">Request</span></span>

<span data-ttu-id="0aca3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0aca3-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="0aca3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0aca3-135">Response</span></span>

<span data-ttu-id="0aca3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0aca3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



