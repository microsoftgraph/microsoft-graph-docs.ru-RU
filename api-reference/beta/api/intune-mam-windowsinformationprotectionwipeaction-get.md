---
title: Получение Виндовсинформатионпротектионвипеактион
description: Чтение свойств и связей объекта Виндовсинформатионпротектионвипеактион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e983d64d46a140451078d97bfac07b3bd4369a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440758"
---
# <a name="get-windowsinformationprotectionwipeaction"></a><span data-ttu-id="b65cc-103">Получение Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="b65cc-103">Get windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="b65cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b65cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b65cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b65cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b65cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b65cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b65cc-107">Чтение свойств и связей объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="b65cc-107">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b65cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b65cc-108">Prerequisites</span></span>
<span data-ttu-id="b65cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b65cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b65cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b65cc-111">Permission type</span></span>|<span data-ttu-id="b65cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b65cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b65cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b65cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b65cc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b65cc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b65cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b65cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b65cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b65cc-116">Not supported.</span></span>|
|<span data-ttu-id="b65cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b65cc-117">Application</span></span>|<span data-ttu-id="b65cc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b65cc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b65cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b65cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b65cc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b65cc-120">Optional query parameters</span></span>
<span data-ttu-id="b65cc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b65cc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b65cc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b65cc-122">Request headers</span></span>
|<span data-ttu-id="b65cc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b65cc-123">Header</span></span>|<span data-ttu-id="b65cc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b65cc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b65cc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b65cc-125">Authorization</span></span>|<span data-ttu-id="b65cc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b65cc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b65cc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b65cc-127">Accept</span></span>|<span data-ttu-id="b65cc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b65cc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b65cc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b65cc-129">Request body</span></span>
<span data-ttu-id="b65cc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b65cc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b65cc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b65cc-131">Response</span></span>
<span data-ttu-id="b65cc-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b65cc-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b65cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b65cc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b65cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b65cc-134">Request</span></span>
<span data-ttu-id="b65cc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b65cc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

### <a name="response"></a><span data-ttu-id="b65cc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b65cc-136">Response</span></span>
<span data-ttu-id="b65cc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b65cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
    "id": "2620a996-a996-2620-96a9-202696a92026",
    "status": "pending",
    "targetedUserId": "Targeted User Id value",
    "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
    "targetedDeviceName": "Targeted Device Name value",
    "targetedDeviceMacAddress": "Targeted Device Mac Address value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
  }
}
```



