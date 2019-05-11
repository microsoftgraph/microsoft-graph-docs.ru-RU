---
title: Получение Граупполициконфигуратионассигнмент
description: Чтение свойств и связей объекта Граупполициконфигуратионассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d98d6692d84fd5c75312fd46cd9c45c7a2a36d5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905135"
---
# <a name="get-grouppolicyconfigurationassignment"></a><span data-ttu-id="42fcf-103">Получение Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="42fcf-103">Get groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="42fcf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42fcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42fcf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42fcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42fcf-106">Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="42fcf-106">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42fcf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42fcf-107">Prerequisites</span></span>
<span data-ttu-id="42fcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42fcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42fcf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42fcf-110">Permission type</span></span>|<span data-ttu-id="42fcf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42fcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42fcf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42fcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42fcf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="42fcf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="42fcf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42fcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42fcf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42fcf-115">Not supported.</span></span>|
|<span data-ttu-id="42fcf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42fcf-116">Application</span></span>|<span data-ttu-id="42fcf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42fcf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42fcf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42fcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42fcf-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42fcf-119">Optional query parameters</span></span>
<span data-ttu-id="42fcf-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42fcf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42fcf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42fcf-121">Request headers</span></span>
|<span data-ttu-id="42fcf-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42fcf-122">Header</span></span>|<span data-ttu-id="42fcf-123">Значение</span><span class="sxs-lookup"><span data-stu-id="42fcf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42fcf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42fcf-124">Authorization</span></span>|<span data-ttu-id="42fcf-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42fcf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42fcf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="42fcf-126">Accept</span></span>|<span data-ttu-id="42fcf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="42fcf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42fcf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42fcf-128">Request body</span></span>
<span data-ttu-id="42fcf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42fcf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42fcf-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="42fcf-130">Response</span></span>
<span data-ttu-id="42fcf-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42fcf-131">If successful, this method returns a `200 OK` response code and [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42fcf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="42fcf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="42fcf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="42fcf-133">Request</span></span>
<span data-ttu-id="42fcf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42fcf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="42fcf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="42fcf-135">Response</span></span>
<span data-ttu-id="42fcf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42fcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
    "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




