---
title: Получение Секуритибаселинекатегористатесуммари
description: Чтение свойств и связей объекта Секуритибаселинекатегористатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1730969b5d72ca71771cc678586b1856f4e7125a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311079"
---
# <a name="get-securitybaselinecategorystatesummary"></a><span data-ttu-id="3d85d-103">Получение Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="3d85d-103">Get securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="3d85d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d85d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d85d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d85d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d85d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d85d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d85d-107">Чтение свойств и связей объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3d85d-107">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d85d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d85d-108">Prerequisites</span></span>
<span data-ttu-id="3d85d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d85d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d85d-111">Permission type</span></span>|<span data-ttu-id="3d85d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d85d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d85d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d85d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d85d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d85d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3d85d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d85d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d85d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d85d-116">Not supported.</span></span>|
|<span data-ttu-id="3d85d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d85d-117">Application</span></span>|<span data-ttu-id="3d85d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d85d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d85d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d85d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d85d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d85d-120">Optional query parameters</span></span>
<span data-ttu-id="3d85d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d85d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d85d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d85d-122">Request headers</span></span>
|<span data-ttu-id="3d85d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d85d-123">Header</span></span>|<span data-ttu-id="3d85d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3d85d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d85d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d85d-125">Authorization</span></span>|<span data-ttu-id="3d85d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d85d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d85d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3d85d-127">Accept</span></span>|<span data-ttu-id="3d85d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3d85d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d85d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d85d-129">Request body</span></span>
<span data-ttu-id="3d85d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d85d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d85d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d85d-131">Response</span></span>
<span data-ttu-id="3d85d-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d85d-132">If successful, this method returns a `200 OK` response code and [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d85d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3d85d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d85d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d85d-134">Request</span></span>
<span data-ttu-id="3d85d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d85d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="3d85d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d85d-136">Response</span></span>
<span data-ttu-id="3d85d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d85d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
    "id": "7a650997-0997-7a65-9709-657a9709657a",
    "secureCount": 11,
    "notSecureCount": 14,
    "unknownCount": 12,
    "errorCount": 10,
    "conflictCount": 13,
    "notApplicableCount": 2,
    "displayName": "Display Name value"
  }
}
```




