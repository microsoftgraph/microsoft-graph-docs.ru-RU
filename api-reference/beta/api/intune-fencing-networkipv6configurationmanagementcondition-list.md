---
title: Список networkIPv6ConfigurationManagementConditions
description: Свойства списка и связей объектов networkIPv6ConfigurationManagementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 64034ece8c2566e6bd4f998e4be3f663e72ee979
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412522"
---
# <a name="list-networkipv6configurationmanagementconditions"></a><span data-ttu-id="fca16-103">Список networkIPv6ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="fca16-103">List networkIPv6ConfigurationManagementConditions</span></span>

> <span data-ttu-id="fca16-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fca16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fca16-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fca16-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fca16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fca16-107">Свойства списка и связей объектов [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="fca16-107">List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fca16-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fca16-108">Prerequisites</span></span>
<span data-ttu-id="fca16-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fca16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fca16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fca16-111">Permission type</span></span>|<span data-ttu-id="fca16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fca16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fca16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fca16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fca16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fca16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fca16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fca16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca16-116">Not supported.</span></span>|
|<span data-ttu-id="fca16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fca16-117">Application</span></span>|<span data-ttu-id="fca16-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fca16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fca16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="fca16-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fca16-120">Request headers</span></span>
|<span data-ttu-id="fca16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fca16-121">Header</span></span>|<span data-ttu-id="fca16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fca16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fca16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fca16-123">Authorization</span></span>|<span data-ttu-id="fca16-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fca16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fca16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fca16-125">Accept</span></span>|<span data-ttu-id="fca16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fca16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fca16-127">Request body</span></span>
<span data-ttu-id="fca16-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fca16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca16-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca16-129">Response</span></span>
<span data-ttu-id="fca16-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fca16-130">If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca16-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fca16-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fca16-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fca16-132">Request</span></span>
<span data-ttu-id="fca16-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fca16-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="fca16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca16-134">Response</span></span>
<span data-ttu-id="fca16-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fca16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
      "id": "25811206-1206-2581-0612-812506128125",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "ipV6Prefix": "Ip V6Prefix value",
      "ipV6Gateway": "Ip V6Gateway value",
      "ipV6DNSServerList": [
        "Ip V6DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```




