---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bcf192a78888ece145c7d60ebcfd887fb873531
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536205"
---
# <a name="list-devicecategories"></a><span data-ttu-id="7e43c-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7e43c-103">List deviceCategories</span></span>

> <span data-ttu-id="7e43c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7e43c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e43c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e43c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e43c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e43c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e43c-107">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7e43c-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e43c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e43c-108">Prerequisites</span></span>
<span data-ttu-id="7e43c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e43c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e43c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e43c-111">Permission type</span></span>|<span data-ttu-id="7e43c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e43c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e43c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e43c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e43c-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7e43c-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7e43c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e43c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7e43c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e43c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e43c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e43c-117">Not supported.</span></span>|
|<span data-ttu-id="7e43c-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e43c-118">Application</span></span>||
| <span data-ttu-id="7e43c-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7e43c-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7e43c-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e43c-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e43c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e43c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="7e43c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e43c-122">Request headers</span></span>

|<span data-ttu-id="7e43c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e43c-123">Header</span></span>|<span data-ttu-id="7e43c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7e43c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e43c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e43c-125">Authorization</span></span>|<span data-ttu-id="7e43c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e43c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e43c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7e43c-127">Accept</span></span>|<span data-ttu-id="7e43c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7e43c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e43c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e43c-129">Request body</span></span>

<span data-ttu-id="7e43c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e43c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e43c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e43c-131">Response</span></span>

<span data-ttu-id="7e43c-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e43c-132">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e43c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7e43c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e43c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e43c-134">Request</span></span>

<span data-ttu-id="7e43c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e43c-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="7e43c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e43c-136">Response</span></span>

<span data-ttu-id="7e43c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e43c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









