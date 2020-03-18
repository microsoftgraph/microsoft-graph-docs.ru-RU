---
title: Список Нетворкманажементкондитионс
description: Список свойств и связей объектов Нетворкманажементкондитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c26f51b70cff597969181966960dbb53b5b693a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804648"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="95fd2-103">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="95fd2-103">List networkManagementConditions</span></span>

> <span data-ttu-id="95fd2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95fd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95fd2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95fd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95fd2-106">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="95fd2-106">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95fd2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95fd2-107">Prerequisites</span></span>
<span data-ttu-id="95fd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95fd2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95fd2-110">Permission type</span></span>|<span data-ttu-id="95fd2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95fd2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95fd2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95fd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95fd2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95fd2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95fd2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95fd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95fd2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95fd2-115">Not supported.</span></span>|
|<span data-ttu-id="95fd2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="95fd2-116">Application</span></span>|<span data-ttu-id="95fd2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95fd2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95fd2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95fd2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="95fd2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95fd2-119">Request headers</span></span>
|<span data-ttu-id="95fd2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95fd2-120">Header</span></span>|<span data-ttu-id="95fd2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95fd2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95fd2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95fd2-122">Authorization</span></span>|<span data-ttu-id="95fd2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95fd2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95fd2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95fd2-124">Accept</span></span>|<span data-ttu-id="95fd2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95fd2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95fd2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95fd2-126">Request body</span></span>
<span data-ttu-id="95fd2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95fd2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95fd2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="95fd2-128">Response</span></span>
<span data-ttu-id="95fd2-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95fd2-129">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95fd2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95fd2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95fd2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95fd2-131">Request</span></span>
<span data-ttu-id="95fd2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95fd2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="95fd2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="95fd2-133">Response</span></span>
<span data-ttu-id="95fd2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95fd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




