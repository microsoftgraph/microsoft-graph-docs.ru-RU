---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f54865cd8156b1661f2312cf0335b99f08dd90be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950293"
---
# <a name="list-devicecategories"></a><span data-ttu-id="a31dd-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a31dd-103">List deviceCategories</span></span>

> <span data-ttu-id="a31dd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a31dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a31dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a31dd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a31dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a31dd-107">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="a31dd-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a31dd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a31dd-108">Prerequisites</span></span>
<span data-ttu-id="a31dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a31dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a31dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a31dd-111">Permission type</span></span>|<span data-ttu-id="a31dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a31dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a31dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a31dd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a31dd-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="a31dd-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a31dd-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a31dd-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a31dd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a31dd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a31dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31dd-117">Not supported.</span></span>|
|<span data-ttu-id="a31dd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a31dd-118">Application</span></span>|<span data-ttu-id="a31dd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31dd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a31dd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a31dd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="a31dd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a31dd-121">Request headers</span></span>

|<span data-ttu-id="a31dd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a31dd-122">Header</span></span>|<span data-ttu-id="a31dd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a31dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a31dd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a31dd-124">Authorization</span></span>|<span data-ttu-id="a31dd-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a31dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a31dd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a31dd-126">Accept</span></span>|<span data-ttu-id="a31dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a31dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31dd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a31dd-128">Request body</span></span>

<span data-ttu-id="a31dd-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a31dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a31dd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a31dd-130">Response</span></span>

<span data-ttu-id="a31dd-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a31dd-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a31dd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a31dd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a31dd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a31dd-133">Request</span></span>

<span data-ttu-id="a31dd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a31dd-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="a31dd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a31dd-135">Response</span></span>

<span data-ttu-id="a31dd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a31dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



