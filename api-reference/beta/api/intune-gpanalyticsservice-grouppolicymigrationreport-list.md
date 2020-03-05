---
title: Список Граупполицимигратионрепортс
description: Список свойств и связей объектов Граупполицимигратионрепорт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d87fe0defd35e5c0623951b8fb8c959248f07ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465487"
---
# <a name="list-grouppolicymigrationreports"></a><span data-ttu-id="c2285-103">Список Граупполицимигратионрепортс</span><span class="sxs-lookup"><span data-stu-id="c2285-103">List groupPolicyMigrationReports</span></span>

<span data-ttu-id="c2285-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2285-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2285-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2285-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2285-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2285-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2285-107">Список свойств и связей объектов [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="c2285-107">List properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2285-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2285-108">Prerequisites</span></span>
<span data-ttu-id="c2285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2285-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2285-111">Permission type</span></span>|<span data-ttu-id="c2285-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2285-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2285-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2285-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2285-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2285-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2285-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2285-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2285-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2285-116">Not supported.</span></span>|
|<span data-ttu-id="c2285-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2285-117">Application</span></span>|<span data-ttu-id="c2285-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2285-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2285-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2285-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="c2285-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2285-120">Request headers</span></span>
|<span data-ttu-id="c2285-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2285-121">Header</span></span>|<span data-ttu-id="c2285-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2285-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2285-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2285-123">Authorization</span></span>|<span data-ttu-id="c2285-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2285-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2285-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2285-125">Accept</span></span>|<span data-ttu-id="c2285-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2285-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2285-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2285-127">Request body</span></span>
<span data-ttu-id="c2285-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2285-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2285-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2285-129">Response</span></span>
<span data-ttu-id="c2285-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2285-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2285-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2285-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2285-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2285-132">Request</span></span>
<span data-ttu-id="c2285-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2285-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
```

### <a name="response"></a><span data-ttu-id="c2285-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2285-134">Response</span></span>
<span data-ttu-id="c2285-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2285-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 805

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
      "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
      "displayName": "Display Name value",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
      "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
      "migrationReadiness": "partial",
      "targetedInActiveDirectory": true,
      "totalSettingsCount": 2,
      "supportedSettingsCount": 6,
      "supportedSettingsPercent": 8
    }
  ]
}
```





