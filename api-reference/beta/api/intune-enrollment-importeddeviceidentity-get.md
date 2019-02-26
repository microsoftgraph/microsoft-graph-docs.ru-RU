---
title: Получение Импортеддевицеидентити
description: Чтение свойств и связей объекта Импортеддевицеидентити.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bac93ae04a5a8e7b2a0edb280a9c6ca79a09394
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141050"
---
# <a name="get-importeddeviceidentity"></a><span data-ttu-id="f89ff-103">Получение Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="f89ff-103">Get importedDeviceIdentity</span></span>

> <span data-ttu-id="f89ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f89ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f89ff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f89ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f89ff-106">Чтение свойств и связей объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f89ff-106">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f89ff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f89ff-107">Prerequisites</span></span>
<span data-ttu-id="f89ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f89ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f89ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f89ff-110">Permission type</span></span>|<span data-ttu-id="f89ff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f89ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f89ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f89ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f89ff-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f89ff-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f89ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f89ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f89ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f89ff-115">Not supported.</span></span>|
|<span data-ttu-id="f89ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f89ff-116">Application</span></span>|<span data-ttu-id="f89ff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f89ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f89ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f89ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f89ff-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f89ff-119">Optional query parameters</span></span>
<span data-ttu-id="f89ff-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f89ff-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f89ff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f89ff-121">Request headers</span></span>
|<span data-ttu-id="f89ff-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f89ff-122">Header</span></span>|<span data-ttu-id="f89ff-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f89ff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f89ff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f89ff-124">Authorization</span></span>|<span data-ttu-id="f89ff-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f89ff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f89ff-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f89ff-126">Accept</span></span>|<span data-ttu-id="f89ff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f89ff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f89ff-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f89ff-128">Request body</span></span>
<span data-ttu-id="f89ff-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f89ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f89ff-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f89ff-130">Response</span></span>
<span data-ttu-id="f89ff-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f89ff-131">If successful, this method returns a `200 OK` response code and [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f89ff-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f89ff-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f89ff-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f89ff-133">Request</span></span>
<span data-ttu-id="f89ff-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f89ff-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="f89ff-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f89ff-135">Response</span></span>
<span data-ttu-id="f89ff-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f89ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
    "@odata.type": "#microsoft.graph.importedDeviceIdentity",
    "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
    "importedDeviceIdentifier": "Imported Device Identifier value",
    "importedDeviceIdentityType": "imei",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "description": "Description value",
    "enrollmentState": "enrolled",
    "platform": "ios"
  }
}
```




