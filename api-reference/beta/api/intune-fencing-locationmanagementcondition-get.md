---
title: Получение Локатионманажементкондитион
description: Чтение свойств и связей объекта Локатионманажементкондитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a737329da35c226f30de2ba11e2e25af5dcf3eb8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072216"
---
# <a name="get-locationmanagementcondition"></a><span data-ttu-id="e638c-103">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="e638c-103">Get locationManagementCondition</span></span>

<span data-ttu-id="e638c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e638c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e638c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e638c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e638c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e638c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e638c-107">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="e638c-107">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e638c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e638c-108">Prerequisites</span></span>
<span data-ttu-id="e638c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e638c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e638c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e638c-111">Permission type</span></span>|<span data-ttu-id="e638c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e638c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e638c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e638c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e638c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e638c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e638c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e638c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e638c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e638c-116">Not supported.</span></span>|
|<span data-ttu-id="e638c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e638c-117">Application</span></span>|<span data-ttu-id="e638c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e638c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e638c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e638c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e638c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e638c-120">Optional query parameters</span></span>
<span data-ttu-id="e638c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e638c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e638c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e638c-122">Request headers</span></span>
|<span data-ttu-id="e638c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e638c-123">Header</span></span>|<span data-ttu-id="e638c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e638c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e638c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e638c-125">Authorization</span></span>|<span data-ttu-id="e638c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e638c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e638c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e638c-127">Accept</span></span>|<span data-ttu-id="e638c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e638c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e638c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e638c-129">Request body</span></span>
<span data-ttu-id="e638c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e638c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e638c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e638c-131">Response</span></span>
<span data-ttu-id="e638c-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e638c-132">If successful, this method returns a `200 OK` response code and [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e638c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e638c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e638c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e638c-134">Request</span></span>
<span data-ttu-id="e638c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e638c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="e638c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e638c-136">Response</span></span>
<span data-ttu-id="e638c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e638c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.locationManagementCondition",
    "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
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
}
```






