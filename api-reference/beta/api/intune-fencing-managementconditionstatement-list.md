---
title: Список Манажементкондитионстатементс
description: Список свойств и связей объектов Манажементкондитионстатемент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 689454a9604e91a1b1015614b72dbfebc70af7c2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804739"
---
# <a name="list-managementconditionstatements"></a><span data-ttu-id="cf972-103">Список Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="cf972-103">List managementConditionStatements</span></span>

> <span data-ttu-id="cf972-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf972-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf972-106">Список свойств и связей объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="cf972-106">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf972-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf972-107">Prerequisites</span></span>
<span data-ttu-id="cf972-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf972-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf972-110">Permission type</span></span>|<span data-ttu-id="cf972-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf972-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf972-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf972-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf972-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf972-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf972-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf972-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf972-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf972-115">Not supported.</span></span>|
|<span data-ttu-id="cf972-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf972-116">Application</span></span>|<span data-ttu-id="cf972-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf972-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf972-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf972-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="cf972-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf972-119">Request headers</span></span>
|<span data-ttu-id="cf972-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf972-120">Header</span></span>|<span data-ttu-id="cf972-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf972-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf972-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf972-122">Authorization</span></span>|<span data-ttu-id="cf972-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf972-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf972-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf972-124">Accept</span></span>|<span data-ttu-id="cf972-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf972-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf972-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf972-126">Request body</span></span>
<span data-ttu-id="cf972-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf972-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf972-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf972-128">Response</span></span>
<span data-ttu-id="cf972-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf972-129">If successful, this method returns a `200 OK` response code and a collection of [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf972-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cf972-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf972-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf972-131">Request</span></span>
<span data-ttu-id="cf972-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf972-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
```

### <a name="response"></a><span data-ttu-id="cf972-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf972-133">Response</span></span>
<span data-ttu-id="cf972-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

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
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




