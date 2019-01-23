---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c27099cdc0e2ffbbc3e0e02cde07b9b4e34ea33c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408315"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="37792-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="37792-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="37792-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37792-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37792-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37792-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37792-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37792-107">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="37792-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37792-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="37792-108">Prerequisites</span></span>

<span data-ttu-id="37792-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="37792-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="37792-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37792-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="37792-111">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="37792-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="37792-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37792-112">Permission type</span></span>|<span data-ttu-id="37792-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37792-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="37792-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37792-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="37792-115">&nbsp;&nbsp; **Приложений**, **книги**или **адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="37792-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="37792-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="37792-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="37792-117">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="37792-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="37792-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="37792-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="37792-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37792-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37792-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37792-120">Not supported.</span></span>|
|<span data-ttu-id="37792-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37792-121">Application</span></span>|<span data-ttu-id="37792-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37792-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37792-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37792-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37792-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37792-124">Optional query parameters</span></span>

<span data-ttu-id="37792-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37792-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37792-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37792-126">Request headers</span></span>

|<span data-ttu-id="37792-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37792-127">Header</span></span>|<span data-ttu-id="37792-128">Значение</span><span class="sxs-lookup"><span data-stu-id="37792-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37792-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="37792-129">Authorization</span></span>|<span data-ttu-id="37792-130">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="37792-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37792-131">Accept</span><span class="sxs-lookup"><span data-stu-id="37792-131">Accept</span></span>|<span data-ttu-id="37792-132">application/json</span><span class="sxs-lookup"><span data-stu-id="37792-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37792-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37792-133">Request body</span></span>

<span data-ttu-id="37792-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37792-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37792-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="37792-135">Response</span></span>

<span data-ttu-id="37792-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37792-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37792-137">Пример</span><span class="sxs-lookup"><span data-stu-id="37792-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="37792-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="37792-138">Request</span></span>

<span data-ttu-id="37792-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37792-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="37792-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="37792-140">Response</span></span>

<span data-ttu-id="37792-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="37792-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



