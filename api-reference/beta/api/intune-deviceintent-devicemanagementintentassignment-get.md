---
title: Получение Девицеманажементинтентассигнмент
description: Чтение свойств и связей объекта Девицеманажементинтентассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 979c49a35fece4c6cb5c8104d96e15a7c77bd85c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43327112"
---
# <a name="get-devicemanagementintentassignment"></a><span data-ttu-id="c0e8b-103">Получение Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="c0e8b-103">Get deviceManagementIntentAssignment</span></span>

<span data-ttu-id="c0e8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0e8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0e8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e8b-107">Чтение свойств и связей объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c0e8b-107">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0e8b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0e8b-108">Prerequisites</span></span>
<span data-ttu-id="c0e8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0e8b-111">Permission type</span></span>|<span data-ttu-id="c0e8b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0e8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0e8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e8b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0e8b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0e8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0e8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-116">Not supported.</span></span>|
|<span data-ttu-id="c0e8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0e8b-117">Application</span></span>|<span data-ttu-id="c0e8b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0e8b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0e8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0e8b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0e8b-120">Optional query parameters</span></span>
<span data-ttu-id="c0e8b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0e8b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0e8b-122">Request headers</span></span>
|<span data-ttu-id="c0e8b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0e8b-123">Header</span></span>|<span data-ttu-id="c0e8b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c0e8b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e8b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0e8b-125">Authorization</span></span>|<span data-ttu-id="c0e8b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e8b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c0e8b-127">Accept</span></span>|<span data-ttu-id="c0e8b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e8b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e8b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0e8b-129">Request body</span></span>
<span data-ttu-id="c0e8b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e8b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0e8b-131">Response</span></span>
<span data-ttu-id="c0e8b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e8b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c0e8b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0e8b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0e8b-134">Request</span></span>
<span data-ttu-id="c0e8b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c0e8b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e8b-136">Response</span></span>
<span data-ttu-id="c0e8b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0e8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
    "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



