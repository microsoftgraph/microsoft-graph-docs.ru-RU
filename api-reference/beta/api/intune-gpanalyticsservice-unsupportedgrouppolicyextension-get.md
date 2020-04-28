---
title: Получение Унсуппортедграупполициекстенсион
description: Чтение свойств и связей объекта Унсуппортедграупполициекстенсион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95dc074bd6a1827b806ab1b4c9fa4c59ddafe7b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454801"
---
# <a name="get-unsupportedgrouppolicyextension"></a><span data-ttu-id="ccfcc-103">Получение Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="ccfcc-103">Get unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="ccfcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccfcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccfcc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccfcc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccfcc-107">Чтение свойств и связей объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="ccfcc-107">Read properties and relationships of the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccfcc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccfcc-108">Prerequisites</span></span>
<span data-ttu-id="ccfcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccfcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccfcc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccfcc-111">Permission type</span></span>|<span data-ttu-id="ccfcc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccfcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccfcc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccfcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccfcc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccfcc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ccfcc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccfcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccfcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-116">Not supported.</span></span>|
|<span data-ttu-id="ccfcc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccfcc-117">Application</span></span>|<span data-ttu-id="ccfcc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccfcc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccfcc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccfcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccfcc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ccfcc-120">Optional query parameters</span></span>
<span data-ttu-id="ccfcc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccfcc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccfcc-122">Request headers</span></span>
|<span data-ttu-id="ccfcc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccfcc-123">Header</span></span>|<span data-ttu-id="ccfcc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ccfcc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccfcc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccfcc-125">Authorization</span></span>|<span data-ttu-id="ccfcc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccfcc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ccfcc-127">Accept</span></span>|<span data-ttu-id="ccfcc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ccfcc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccfcc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccfcc-129">Request body</span></span>
<span data-ttu-id="ccfcc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccfcc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccfcc-131">Response</span></span>
<span data-ttu-id="ccfcc-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-132">If successful, this method returns a `200 OK` response code and [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccfcc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ccfcc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccfcc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccfcc-134">Request</span></span>
<span data-ttu-id="ccfcc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

### <a name="response"></a><span data-ttu-id="ccfcc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfcc-136">Response</span></span>
<span data-ttu-id="ccfcc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccfcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



