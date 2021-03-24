---
title: Get managedAppOperation
description: Чтение свойств и связей объекта managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2befca56075c2b29e05ac57471d29b34f6c7031e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149291"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="52a01-103">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="52a01-103">Get managedAppOperation</span></span>

<span data-ttu-id="52a01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52a01-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52a01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52a01-107">Чтение свойств и связей объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="52a01-107">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52a01-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="52a01-108">Prerequisites</span></span>
<span data-ttu-id="52a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52a01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52a01-111">Permission type</span></span>|<span data-ttu-id="52a01-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52a01-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52a01-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52a01-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52a01-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52a01-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52a01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52a01-116">Not supported.</span></span>|
|<span data-ttu-id="52a01-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="52a01-117">Application</span></span>|<span data-ttu-id="52a01-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52a01-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52a01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52a01-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52a01-120">Optional query parameters</span></span>
<span data-ttu-id="52a01-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52a01-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52a01-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52a01-122">Request headers</span></span>
|<span data-ttu-id="52a01-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52a01-123">Header</span></span>|<span data-ttu-id="52a01-124">Значение</span><span class="sxs-lookup"><span data-stu-id="52a01-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52a01-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="52a01-125">Authorization</span></span>|<span data-ttu-id="52a01-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52a01-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52a01-127">Accept</span><span class="sxs-lookup"><span data-stu-id="52a01-127">Accept</span></span>|<span data-ttu-id="52a01-128">application/json</span><span class="sxs-lookup"><span data-stu-id="52a01-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52a01-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52a01-129">Request body</span></span>
<span data-ttu-id="52a01-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52a01-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52a01-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a01-131">Response</span></span>
<span data-ttu-id="52a01-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52a01-132">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52a01-133">Пример</span><span class="sxs-lookup"><span data-stu-id="52a01-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="52a01-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="52a01-134">Request</span></span>
<span data-ttu-id="52a01-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52a01-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="52a01-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a01-136">Response</span></span>
<span data-ttu-id="52a01-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52a01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppOperation",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "State value",
    "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
    "version": "Version value"
  }
}
```




