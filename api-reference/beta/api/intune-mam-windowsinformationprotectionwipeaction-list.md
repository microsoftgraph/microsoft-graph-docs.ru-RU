---
title: Список Виндовсинформатионпротектионвипеактионс
description: Список свойств и связей объектов Виндовсинформатионпротектионвипеактион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9ed778fb3978f9b5cf76a249b1e7198ad3b55ee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285634"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="687a1-103">Список Виндовсинформатионпротектионвипеактионс</span><span class="sxs-lookup"><span data-stu-id="687a1-103">List windowsInformationProtectionWipeActions</span></span>

<span data-ttu-id="687a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="687a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="687a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="687a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="687a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="687a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="687a1-107">Список свойств и связей объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="687a1-107">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="687a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="687a1-108">Prerequisites</span></span>
<span data-ttu-id="687a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="687a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="687a1-111">Permission type</span></span>|<span data-ttu-id="687a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="687a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="687a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="687a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="687a1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="687a1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="687a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="687a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="687a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="687a1-116">Not supported.</span></span>|
|<span data-ttu-id="687a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="687a1-117">Application</span></span>|<span data-ttu-id="687a1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="687a1-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="687a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="687a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="687a1-120">Request headers</span></span>
|<span data-ttu-id="687a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="687a1-121">Header</span></span>|<span data-ttu-id="687a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="687a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="687a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="687a1-123">Authorization</span></span>|<span data-ttu-id="687a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="687a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="687a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="687a1-125">Accept</span></span>|<span data-ttu-id="687a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="687a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="687a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="687a1-127">Request body</span></span>
<span data-ttu-id="687a1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="687a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="687a1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="687a1-129">Response</span></span>
<span data-ttu-id="687a1-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="687a1-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="687a1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="687a1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="687a1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="687a1-132">Request</span></span>
<span data-ttu-id="687a1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="687a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="687a1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="687a1-134">Response</span></span>
<span data-ttu-id="687a1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="687a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




