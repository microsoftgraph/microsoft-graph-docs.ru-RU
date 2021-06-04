---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47362ae05da50c418c908e94ac0f7790f5aa85b0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753938"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="821cf-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="821cf-103">List deviceConfigurationAssignments</span></span>

<span data-ttu-id="821cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="821cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="821cf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="821cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="821cf-106">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="821cf-106">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="821cf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="821cf-107">Prerequisites</span></span>
<span data-ttu-id="821cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="821cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="821cf-110">Permission type</span></span>|<span data-ttu-id="821cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="821cf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="821cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="821cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="821cf-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="821cf-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="821cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="821cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="821cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="821cf-115">Not supported.</span></span>|
|<span data-ttu-id="821cf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="821cf-116">Application</span></span>|<span data-ttu-id="821cf-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="821cf-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="821cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="821cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="821cf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="821cf-119">Request headers</span></span>
|<span data-ttu-id="821cf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="821cf-120">Header</span></span>|<span data-ttu-id="821cf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="821cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="821cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="821cf-122">Authorization</span></span>|<span data-ttu-id="821cf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="821cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="821cf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="821cf-124">Accept</span></span>|<span data-ttu-id="821cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="821cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="821cf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="821cf-126">Request body</span></span>
<span data-ttu-id="821cf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="821cf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="821cf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="821cf-128">Response</span></span>
<span data-ttu-id="821cf-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="821cf-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821cf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="821cf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="821cf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="821cf-131">Request</span></span>
<span data-ttu-id="821cf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="821cf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="821cf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="821cf-133">Response</span></span>
<span data-ttu-id="821cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="821cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




