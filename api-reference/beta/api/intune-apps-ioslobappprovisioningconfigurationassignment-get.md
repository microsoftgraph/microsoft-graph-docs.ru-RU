---
title: Получение Иослобапппровисионингконфигуратионассигнмент
description: Чтение свойств и связей объекта Иослобапппровисионингконфигуратионассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a930d78ee8e234fc6a548af86c9057360724362d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793397"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="4146b-103">Получение Иослобапппровисионингконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="4146b-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="4146b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4146b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4146b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4146b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4146b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4146b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4146b-107">Чтение свойств и связей объекта [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4146b-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4146b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4146b-108">Prerequisites</span></span>
<span data-ttu-id="4146b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4146b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4146b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4146b-111">Permission type</span></span>|<span data-ttu-id="4146b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4146b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4146b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4146b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4146b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4146b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4146b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4146b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4146b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4146b-116">Not supported.</span></span>|
|<span data-ttu-id="4146b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4146b-117">Application</span></span>|<span data-ttu-id="4146b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4146b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4146b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4146b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4146b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4146b-120">Optional query parameters</span></span>
<span data-ttu-id="4146b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4146b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4146b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4146b-122">Request headers</span></span>
|<span data-ttu-id="4146b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4146b-123">Header</span></span>|<span data-ttu-id="4146b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4146b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4146b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4146b-125">Authorization</span></span>|<span data-ttu-id="4146b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4146b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4146b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4146b-127">Accept</span></span>|<span data-ttu-id="4146b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4146b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4146b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4146b-129">Request body</span></span>
<span data-ttu-id="4146b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4146b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4146b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4146b-131">Response</span></span>
<span data-ttu-id="4146b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [иослобапппровисионингконфигуратионассигнмент](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4146b-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4146b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4146b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4146b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4146b-134">Request</span></span>
<span data-ttu-id="4146b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4146b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="4146b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4146b-136">Response</span></span>
<span data-ttu-id="4146b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4146b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```



