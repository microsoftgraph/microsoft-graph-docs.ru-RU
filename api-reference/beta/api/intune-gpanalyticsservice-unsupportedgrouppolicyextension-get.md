---
title: Получение Унсуппортедграупполициекстенсион
description: Чтение свойств и связей объекта Унсуппортедграупполициекстенсион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5012e3817228bac382b1b81cf8f5a2d574c9b634
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161335"
---
# <a name="get-unsupportedgrouppolicyextension"></a><span data-ttu-id="a8dbf-103">Получение Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="a8dbf-103">Get unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="a8dbf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8dbf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8dbf-106">Чтение свойств и связей объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="a8dbf-106">Read properties and relationships of the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8dbf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8dbf-107">Prerequisites</span></span>
<span data-ttu-id="a8dbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8dbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8dbf-110">Permission type</span></span>|<span data-ttu-id="a8dbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8dbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8dbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8dbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8dbf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8dbf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8dbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8dbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8dbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-115">Not supported.</span></span>|
|<span data-ttu-id="a8dbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8dbf-116">Application</span></span>|<span data-ttu-id="a8dbf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8dbf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8dbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8dbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8dbf-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8dbf-119">Optional query parameters</span></span>
<span data-ttu-id="a8dbf-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8dbf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8dbf-121">Request headers</span></span>
|<span data-ttu-id="a8dbf-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8dbf-122">Header</span></span>|<span data-ttu-id="a8dbf-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a8dbf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8dbf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8dbf-124">Authorization</span></span>|<span data-ttu-id="a8dbf-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8dbf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a8dbf-126">Accept</span></span>|<span data-ttu-id="a8dbf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a8dbf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8dbf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8dbf-128">Request body</span></span>
<span data-ttu-id="a8dbf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8dbf-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8dbf-130">Response</span></span>
<span data-ttu-id="a8dbf-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-131">If successful, this method returns a `200 OK` response code and [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8dbf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a8dbf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8dbf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8dbf-133">Request</span></span>
<span data-ttu-id="a8dbf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

### <a name="response"></a><span data-ttu-id="a8dbf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8dbf-135">Response</span></span>
<span data-ttu-id="a8dbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8dbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": {
    "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
    "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
    "settingScope": "device",
    "namespaceUrl": "https://example.com/namespaceUrl/",
    "extensionType": "Extension Type value",
    "nodeName": "Node Name value"
  }
}
```





