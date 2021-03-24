---
title: List deviceConfigurationConflictSummaries
description: Список свойств и связей объектов deviceConfigurationConflictSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9c789b0872b69443ac139c78cd1cfeef5e9be79f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131703"
---
# <a name="list-deviceconfigurationconflictsummaries"></a><span data-ttu-id="bc6fa-103">List deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="bc6fa-103">List deviceConfigurationConflictSummaries</span></span>

<span data-ttu-id="bc6fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc6fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc6fa-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc6fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc6fa-107">Список свойств и связей [объектов deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)</span><span class="sxs-lookup"><span data-stu-id="bc6fa-107">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc6fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc6fa-108">Prerequisites</span></span>
<span data-ttu-id="bc6fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc6fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc6fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc6fa-111">Permission type</span></span>|<span data-ttu-id="bc6fa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc6fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc6fa-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc6fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc6fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc6fa-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc6fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc6fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-116">Not supported.</span></span>|
|<span data-ttu-id="bc6fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc6fa-117">Application</span></span>|<span data-ttu-id="bc6fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc6fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc6fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc6fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="bc6fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bc6fa-120">Request headers</span></span>
|<span data-ttu-id="bc6fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc6fa-121">Header</span></span>|<span data-ttu-id="bc6fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc6fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc6fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc6fa-123">Authorization</span></span>|<span data-ttu-id="bc6fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc6fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc6fa-125">Accept</span></span>|<span data-ttu-id="bc6fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc6fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc6fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc6fa-127">Request body</span></span>
<span data-ttu-id="bc6fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc6fa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc6fa-129">Response</span></span>
<span data-ttu-id="bc6fa-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc6fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bc6fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc6fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc6fa-132">Request</span></span>
<span data-ttu-id="bc6fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### <a name="response"></a><span data-ttu-id="bc6fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc6fa-134">Response</span></span>
<span data-ttu-id="bc6fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc6fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
      "conflictingDeviceConfigurations": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value",
          "sourceType": "deviceIntent"
        }
      ],
      "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
      "contributingSettings": [
        "Contributing Settings value"
      ],
      "deviceCheckinsImpacted": 6
    }
  ]
}
```




