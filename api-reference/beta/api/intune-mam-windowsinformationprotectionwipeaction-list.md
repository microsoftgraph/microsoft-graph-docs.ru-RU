---
title: Список Виндовсинформатионпротектионвипеактионс
description: Список свойств и связей объектов Виндовсинформатионпротектионвипеактион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 113763f043c08190130d55fd937d3ab97af73c55
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017502"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="37dab-103">Список Виндовсинформатионпротектионвипеактионс</span><span class="sxs-lookup"><span data-stu-id="37dab-103">List windowsInformationProtectionWipeActions</span></span>

<span data-ttu-id="37dab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37dab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37dab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37dab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37dab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37dab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37dab-107">Список свойств и связей объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="37dab-107">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37dab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37dab-108">Prerequisites</span></span>
<span data-ttu-id="37dab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37dab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37dab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37dab-111">Permission type</span></span>|<span data-ttu-id="37dab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37dab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37dab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37dab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37dab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37dab-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="37dab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37dab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37dab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37dab-116">Not supported.</span></span>|
|<span data-ttu-id="37dab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37dab-117">Application</span></span>|<span data-ttu-id="37dab-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="37dab-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37dab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37dab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="37dab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37dab-120">Request headers</span></span>
|<span data-ttu-id="37dab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37dab-121">Header</span></span>|<span data-ttu-id="37dab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37dab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37dab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37dab-123">Authorization</span></span>|<span data-ttu-id="37dab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37dab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37dab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37dab-125">Accept</span></span>|<span data-ttu-id="37dab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37dab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37dab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37dab-127">Request body</span></span>
<span data-ttu-id="37dab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37dab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37dab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="37dab-129">Response</span></span>
<span data-ttu-id="37dab-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37dab-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37dab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="37dab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37dab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37dab-132">Request</span></span>
<span data-ttu-id="37dab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37dab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="37dab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37dab-134">Response</span></span>
<span data-ttu-id="37dab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37dab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "2620a996-a996-2620-96a9-202696a92026",
      "status": "pending",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
    }
  ]
}
```






