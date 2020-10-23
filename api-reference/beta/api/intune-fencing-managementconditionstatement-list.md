---
title: Список Манажементкондитионстатементс
description: Список свойств и связей объектов Манажементкондитионстатемент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a0d1764b6efe20b5ec3ecca3fec624af1702110
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723201"
---
# <a name="list-managementconditionstatements"></a><span data-ttu-id="4ba73-103">Список Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="4ba73-103">List managementConditionStatements</span></span>

<span data-ttu-id="4ba73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ba73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ba73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ba73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ba73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ba73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ba73-107">Список свойств и связей объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="4ba73-107">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ba73-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ba73-108">Prerequisites</span></span>
<span data-ttu-id="4ba73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba73-111">Permission type</span></span>|<span data-ttu-id="4ba73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ba73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ba73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ba73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ba73-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ba73-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ba73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ba73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ba73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ba73-116">Not supported.</span></span>|
|<span data-ttu-id="4ba73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ba73-117">Application</span></span>|<span data-ttu-id="4ba73-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ba73-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ba73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ba73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="4ba73-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ba73-120">Request headers</span></span>
|<span data-ttu-id="4ba73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ba73-121">Header</span></span>|<span data-ttu-id="4ba73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ba73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ba73-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ba73-123">Authorization</span></span>|<span data-ttu-id="4ba73-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ba73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ba73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ba73-125">Accept</span></span>|<span data-ttu-id="4ba73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ba73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ba73-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ba73-127">Request body</span></span>
<span data-ttu-id="4ba73-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ba73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba73-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ba73-129">Response</span></span>
<span data-ttu-id="4ba73-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ba73-130">If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba73-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4ba73-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ba73-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ba73-132">Request</span></span>
<span data-ttu-id="4ba73-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ba73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
```

### <a name="response"></a><span data-ttu-id="4ba73-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ba73-134">Response</span></span>
<span data-ttu-id="4ba73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ba73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpressionString",
        "value": "Value value"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





