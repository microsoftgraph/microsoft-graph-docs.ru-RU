---
title: Перечисление объектов deviceCategory
description: Список свойств и связей объектов deviceCategory.
ms.openlocfilehash: 826310d9ba694fe5cfd2e8966bd8545fa3fc042a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028275"
---
# <a name="list-devicecategories"></a><span data-ttu-id="1cc1e-103">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1cc1e-103">List deviceCategories</span></span>

> <span data-ttu-id="1cc1e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cc1e-105">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1cc1e-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cc1e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1cc1e-106">Prerequisites</span></span>
<span data-ttu-id="1cc1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cc1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cc1e-109">Permission type</span></span>|<span data-ttu-id="1cc1e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cc1e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cc1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cc1e-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1cc1e-112">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="1cc1e-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1cc1e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cc1e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1cc1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cc1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cc1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-115">Not supported.</span></span>|
|<span data-ttu-id="1cc1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cc1e-116">Application</span></span>|<span data-ttu-id="1cc1e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cc1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cc1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="1cc1e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cc1e-119">Request headers</span></span>
|<span data-ttu-id="1cc1e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cc1e-120">Header</span></span>|<span data-ttu-id="1cc1e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1cc1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cc1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc1e-122">Authorization</span></span>|<span data-ttu-id="1cc1e-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cc1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cc1e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1cc1e-124">Accept</span></span>|<span data-ttu-id="1cc1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cc1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cc1e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cc1e-126">Request body</span></span>
<span data-ttu-id="1cc1e-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc1e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cc1e-128">Response</span></span>
<span data-ttu-id="1cc1e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cc1e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1cc1e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cc1e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cc1e-131">Request</span></span>
<span data-ttu-id="1cc1e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cc1e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="1cc1e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cc1e-133">Response</span></span>
<span data-ttu-id="1cc1e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1cc1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



