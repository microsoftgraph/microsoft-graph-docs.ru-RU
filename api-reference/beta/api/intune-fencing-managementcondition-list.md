---
title: Список Манажементкондитионс
description: Список свойств и связей объектов Манажементкондитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fdc1c9b6599b1991a48b795b3085f4425549a30
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905401"
---
# <a name="list-managementconditions"></a><span data-ttu-id="5d021-103">Список Манажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="5d021-103">List managementConditions</span></span>

> <span data-ttu-id="5d021-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d021-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d021-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d021-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d021-106">Список свойств и связей объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5d021-106">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d021-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5d021-107">Prerequisites</span></span>
<span data-ttu-id="5d021-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d021-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d021-110">Permission type</span></span>|<span data-ttu-id="5d021-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d021-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d021-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d021-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d021-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d021-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5d021-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d021-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d021-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d021-115">Not supported.</span></span>|
|<span data-ttu-id="5d021-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d021-116">Application</span></span>|<span data-ttu-id="5d021-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d021-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d021-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d021-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="5d021-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d021-119">Request headers</span></span>
|<span data-ttu-id="5d021-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d021-120">Header</span></span>|<span data-ttu-id="5d021-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5d021-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d021-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d021-122">Authorization</span></span>|<span data-ttu-id="5d021-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d021-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d021-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5d021-124">Accept</span></span>|<span data-ttu-id="5d021-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d021-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d021-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d021-126">Request body</span></span>
<span data-ttu-id="5d021-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d021-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d021-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d021-128">Response</span></span>
<span data-ttu-id="5d021-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d021-129">If successful, this method returns a `200 OK` response code and a collection of [managementCondition](../resources/intune-fencing-managementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d021-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5d021-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d021-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d021-131">Request</span></span>
<span data-ttu-id="5d021-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d021-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="5d021-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d021-133">Response</span></span>
<span data-ttu-id="5d021-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d021-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
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




