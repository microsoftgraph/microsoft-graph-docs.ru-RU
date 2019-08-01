---
title: Get deviceConfigurationAssignment
description: Чтение свойств и связей объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 978c4abe5f1e088ae16cd91f5b6ea7ec76f3be2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017617"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="9f311-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9f311-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="9f311-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f311-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f311-105">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f311-105">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f311-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9f311-106">Prerequisites</span></span>
<span data-ttu-id="9f311-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f311-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f311-109">Permission type</span></span>|<span data-ttu-id="9f311-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f311-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f311-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f311-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f311-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f311-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f311-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f311-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f311-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f311-114">Not supported.</span></span>|
|<span data-ttu-id="9f311-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f311-115">Application</span></span>|<span data-ttu-id="9f311-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f311-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f311-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f311-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f311-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f311-118">Optional query parameters</span></span>
<span data-ttu-id="9f311-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f311-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f311-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f311-120">Request headers</span></span>
|<span data-ttu-id="9f311-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f311-121">Header</span></span>|<span data-ttu-id="9f311-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f311-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f311-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f311-123">Authorization</span></span>|<span data-ttu-id="9f311-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f311-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f311-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f311-125">Accept</span></span>|<span data-ttu-id="9f311-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f311-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f311-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f311-127">Request body</span></span>
<span data-ttu-id="9f311-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f311-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f311-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f311-129">Response</span></span>
<span data-ttu-id="9f311-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f311-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f311-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9f311-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f311-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f311-132">Request</span></span>
<span data-ttu-id="9f311-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f311-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="9f311-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f311-134">Response</span></span>
<span data-ttu-id="9f311-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f311-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



