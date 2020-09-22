---
title: Получение Девицеманажементсеттингкатегори
description: Чтение свойств и связей объекта Девицеманажементсеттингкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d799e5079bf0b0780f88ad71629b1cea94fcd409
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986667"
---
# <a name="get-devicemanagementsettingcategory"></a><span data-ttu-id="97f59-103">Получение Девицеманажементсеттингкатегори</span><span class="sxs-lookup"><span data-stu-id="97f59-103">Get deviceManagementSettingCategory</span></span>

<span data-ttu-id="97f59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97f59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97f59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97f59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97f59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97f59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97f59-107">Чтение свойств и связей объекта [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="97f59-107">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97f59-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97f59-108">Prerequisites</span></span>
<span data-ttu-id="97f59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97f59-111">Permission type</span></span>|<span data-ttu-id="97f59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97f59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97f59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97f59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97f59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97f59-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97f59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97f59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97f59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97f59-116">Not supported.</span></span>|
|<span data-ttu-id="97f59-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97f59-117">Application</span></span>|<span data-ttu-id="97f59-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97f59-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97f59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97f59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97f59-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="97f59-120">Optional query parameters</span></span>
<span data-ttu-id="97f59-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97f59-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97f59-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97f59-122">Request headers</span></span>
|<span data-ttu-id="97f59-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97f59-123">Header</span></span>|<span data-ttu-id="97f59-124">Значение</span><span class="sxs-lookup"><span data-stu-id="97f59-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97f59-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f59-125">Authorization</span></span>|<span data-ttu-id="97f59-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97f59-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97f59-127">Accept</span><span class="sxs-lookup"><span data-stu-id="97f59-127">Accept</span></span>|<span data-ttu-id="97f59-128">application/json</span><span class="sxs-lookup"><span data-stu-id="97f59-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97f59-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97f59-129">Request body</span></span>
<span data-ttu-id="97f59-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97f59-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97f59-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="97f59-131">Response</span></span>
<span data-ttu-id="97f59-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97f59-132">If successful, this method returns a `200 OK` response code and [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97f59-133">Пример</span><span class="sxs-lookup"><span data-stu-id="97f59-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="97f59-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="97f59-134">Request</span></span>
<span data-ttu-id="97f59-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97f59-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="97f59-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="97f59-136">Response</span></span>
<span data-ttu-id="97f59-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97f59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
    "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
    "displayName": "Display Name value",
    "hasRequiredSetting": true
  }
}
```






