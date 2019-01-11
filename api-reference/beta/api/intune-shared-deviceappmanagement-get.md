---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 27026a7fdbb06f4cbcad20498081b0f2b562d51e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890925"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="eef9e-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="eef9e-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="eef9e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eef9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eef9e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eef9e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eef9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eef9e-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="eef9e-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eef9e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="eef9e-108">Prerequisites</span></span>

<span data-ttu-id="eef9e-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="eef9e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="eef9e-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef9e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="eef9e-111">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="eef9e-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="eef9e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eef9e-112">Permission type</span></span>|<span data-ttu-id="eef9e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eef9e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="eef9e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eef9e-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="eef9e-115">&nbsp;&nbsp; **Приложений**, **книги**или **адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="eef9e-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="eef9e-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="eef9e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="eef9e-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="eef9e-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="eef9e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eef9e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="eef9e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eef9e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef9e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef9e-120">Not supported.</span></span>|
|<span data-ttu-id="eef9e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eef9e-121">Application</span></span>|<span data-ttu-id="eef9e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef9e-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef9e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eef9e-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eef9e-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eef9e-124">Optional query parameters</span></span>

<span data-ttu-id="eef9e-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eef9e-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eef9e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eef9e-126">Request headers</span></span>

|<span data-ttu-id="eef9e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eef9e-127">Header</span></span>|<span data-ttu-id="eef9e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="eef9e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef9e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="eef9e-129">Authorization</span></span>|<span data-ttu-id="eef9e-130">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eef9e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef9e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="eef9e-131">Accept</span></span>|<span data-ttu-id="eef9e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="eef9e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef9e-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eef9e-133">Request body</span></span>

<span data-ttu-id="eef9e-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eef9e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eef9e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="eef9e-135">Response</span></span>

<span data-ttu-id="eef9e-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eef9e-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef9e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="eef9e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="eef9e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="eef9e-138">Request</span></span>

<span data-ttu-id="eef9e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eef9e-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="eef9e-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="eef9e-140">Response</span></span>

<span data-ttu-id="eef9e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eef9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



