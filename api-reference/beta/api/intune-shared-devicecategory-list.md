---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9f3b484a3a518028e826f34092e7295a8a9d7d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868532"
---
# <a name="list-devicecategories"></a><span data-ttu-id="05ea1-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="05ea1-103">List deviceCategories</span></span>

> <span data-ttu-id="05ea1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05ea1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05ea1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ea1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05ea1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05ea1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05ea1-107">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="05ea1-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05ea1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05ea1-108">Prerequisites</span></span>
<span data-ttu-id="05ea1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05ea1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ea1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05ea1-111">Permission type</span></span>|<span data-ttu-id="05ea1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05ea1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05ea1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05ea1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05ea1-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="05ea1-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="05ea1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="05ea1-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="05ea1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05ea1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05ea1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ea1-117">Not supported.</span></span>|
|<span data-ttu-id="05ea1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05ea1-118">Application</span></span>|<span data-ttu-id="05ea1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ea1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05ea1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05ea1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="05ea1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05ea1-121">Request headers</span></span>

|<span data-ttu-id="05ea1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05ea1-122">Header</span></span>|<span data-ttu-id="05ea1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="05ea1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05ea1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05ea1-124">Authorization</span></span>|<span data-ttu-id="05ea1-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05ea1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05ea1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="05ea1-126">Accept</span></span>|<span data-ttu-id="05ea1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05ea1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ea1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05ea1-128">Request body</span></span>

<span data-ttu-id="05ea1-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05ea1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05ea1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="05ea1-130">Response</span></span>

<span data-ttu-id="05ea1-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05ea1-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05ea1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="05ea1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="05ea1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="05ea1-133">Request</span></span>

<span data-ttu-id="05ea1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05ea1-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="05ea1-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="05ea1-135">Response</span></span>

<span data-ttu-id="05ea1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05ea1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



