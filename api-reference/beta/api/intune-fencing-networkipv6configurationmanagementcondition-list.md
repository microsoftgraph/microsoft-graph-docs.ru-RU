---
title: Список networkIPv6ConfigurationManagementConditions
description: Список свойств и связей объектов networkIPv6ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1450656360654dc4e46899adb57a308f00dbd44b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984690"
---
# <a name="list-networkipv6configurationmanagementconditions"></a><span data-ttu-id="634a3-103">Список networkIPv6ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="634a3-103">List networkIPv6ConfigurationManagementConditions</span></span>

> <span data-ttu-id="634a3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="634a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="634a3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="634a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="634a3-106">Список свойств и связей объектов [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="634a3-106">List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="634a3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="634a3-107">Prerequisites</span></span>
<span data-ttu-id="634a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="634a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="634a3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="634a3-110">Permission type</span></span>|<span data-ttu-id="634a3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="634a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="634a3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="634a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="634a3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="634a3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="634a3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="634a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="634a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="634a3-115">Not supported.</span></span>|
|<span data-ttu-id="634a3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="634a3-116">Application</span></span>|<span data-ttu-id="634a3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="634a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="634a3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="634a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="634a3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="634a3-119">Request headers</span></span>
|<span data-ttu-id="634a3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="634a3-120">Header</span></span>|<span data-ttu-id="634a3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="634a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="634a3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="634a3-122">Authorization</span></span>|<span data-ttu-id="634a3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="634a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="634a3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="634a3-124">Accept</span></span>|<span data-ttu-id="634a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="634a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="634a3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="634a3-126">Request body</span></span>
<span data-ttu-id="634a3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="634a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="634a3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="634a3-128">Response</span></span>
<span data-ttu-id="634a3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="634a3-129">If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="634a3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="634a3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="634a3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="634a3-131">Request</span></span>
<span data-ttu-id="634a3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="634a3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="634a3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="634a3-133">Response</span></span>
<span data-ttu-id="634a3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="634a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





