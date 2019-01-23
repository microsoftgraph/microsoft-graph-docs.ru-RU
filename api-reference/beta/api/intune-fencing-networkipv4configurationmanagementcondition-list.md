---
title: Список networkIPv4ConfigurationManagementConditions
description: Свойства списка и связей объектов networkIPv4ConfigurationManagementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa445b2e03159da71831227aece3dfce64fea02c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412571"
---
# <a name="list-networkipv4configurationmanagementconditions"></a><span data-ttu-id="07d36-103">Список networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="07d36-103">List networkIPv4ConfigurationManagementConditions</span></span>

> <span data-ttu-id="07d36-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07d36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07d36-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07d36-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07d36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d36-107">Свойства списка и связей объектов [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="07d36-107">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07d36-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="07d36-108">Prerequisites</span></span>
<span data-ttu-id="07d36-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07d36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d36-111">Permission type</span></span>|<span data-ttu-id="07d36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07d36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07d36-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="07d36-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="07d36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07d36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d36-116">Not supported.</span></span>|
|<span data-ttu-id="07d36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d36-117">Application</span></span>|<span data-ttu-id="07d36-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07d36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="07d36-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d36-120">Request headers</span></span>
|<span data-ttu-id="07d36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07d36-121">Header</span></span>|<span data-ttu-id="07d36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07d36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d36-123">Authorization</span></span>|<span data-ttu-id="07d36-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="07d36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07d36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07d36-125">Accept</span></span>|<span data-ttu-id="07d36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07d36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07d36-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d36-127">Request body</span></span>
<span data-ttu-id="07d36-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07d36-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07d36-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d36-129">Response</span></span>
<span data-ttu-id="07d36-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07d36-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d36-131">Пример</span><span class="sxs-lookup"><span data-stu-id="07d36-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="07d36-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d36-132">Request</span></span>
<span data-ttu-id="07d36-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d36-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="07d36-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d36-134">Response</span></span>
<span data-ttu-id="07d36-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07d36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
      "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "ipV4Prefix": "Ip V4Prefix value",
      "ipV4Gateway": "Ip V4Gateway value",
      "ipV4DHCPServer": "Ip V4DHCPServer value",
      "ipV4DNSServerList": [
        "Ip V4DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```




