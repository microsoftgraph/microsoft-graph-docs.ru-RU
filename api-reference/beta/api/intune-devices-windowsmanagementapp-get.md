---
title: Получение windowsManagementApp
description: Чтение свойств и связей объекта windowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5524ddba642db143b53e417b01f430a9c57d1ff8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321620"
---
# <a name="get-windowsmanagementapp"></a><span data-ttu-id="e5743-103">Получение windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="e5743-103">Get windowsManagementApp</span></span>

<span data-ttu-id="e5743-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5743-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5743-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5743-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5743-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5743-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5743-107">Чтение свойств и связей объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e5743-107">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5743-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5743-108">Prerequisites</span></span>
<span data-ttu-id="e5743-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5743-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5743-111">Permission type</span></span>|<span data-ttu-id="e5743-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5743-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5743-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5743-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5743-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5743-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e5743-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5743-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5743-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5743-116">Not supported.</span></span>|
|<span data-ttu-id="e5743-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5743-117">Application</span></span>|<span data-ttu-id="e5743-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5743-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5743-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5743-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5743-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5743-120">Optional query parameters</span></span>
<span data-ttu-id="e5743-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5743-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5743-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5743-122">Request headers</span></span>
|<span data-ttu-id="e5743-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5743-123">Header</span></span>|<span data-ttu-id="e5743-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e5743-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5743-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5743-125">Authorization</span></span>|<span data-ttu-id="e5743-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5743-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5743-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e5743-127">Accept</span></span>|<span data-ttu-id="e5743-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e5743-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5743-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5743-129">Request body</span></span>
<span data-ttu-id="e5743-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5743-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5743-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5743-131">Response</span></span>
<span data-ttu-id="e5743-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5743-132">If successful, this method returns a `200 OK` response code and [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5743-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e5743-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5743-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5743-134">Request</span></span>
<span data-ttu-id="e5743-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5743-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
```

### <a name="response"></a><span data-ttu-id="e5743-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5743-136">Response</span></span>
<span data-ttu-id="e5743-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5743-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementApp",
    "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
    "availableVersion": "Available Version value"
  }
}
```



