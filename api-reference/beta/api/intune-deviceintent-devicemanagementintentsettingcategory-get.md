---
title: Get deviceManagementIntentSettingCategory
description: Чтение свойств и связей объекта deviceManagementIntentSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea4b2744b53e778dd02b4659a6eb33e540441242
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130940"
---
# <a name="get-devicemanagementintentsettingcategory"></a><span data-ttu-id="25ee2-103">Get deviceManagementIntentSettingCategory</span><span class="sxs-lookup"><span data-stu-id="25ee2-103">Get deviceManagementIntentSettingCategory</span></span>

<span data-ttu-id="25ee2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25ee2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25ee2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25ee2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25ee2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25ee2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25ee2-107">Чтение свойств и связей [объекта deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="25ee2-107">Read properties and relationships of the [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25ee2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25ee2-108">Prerequisites</span></span>
<span data-ttu-id="25ee2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25ee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ee2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25ee2-111">Permission type</span></span>|<span data-ttu-id="25ee2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25ee2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25ee2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25ee2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25ee2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ee2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25ee2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25ee2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25ee2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25ee2-116">Not supported.</span></span>|
|<span data-ttu-id="25ee2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="25ee2-117">Application</span></span>|<span data-ttu-id="25ee2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ee2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25ee2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25ee2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25ee2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25ee2-120">Optional query parameters</span></span>
<span data-ttu-id="25ee2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25ee2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25ee2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25ee2-122">Request headers</span></span>
|<span data-ttu-id="25ee2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25ee2-123">Header</span></span>|<span data-ttu-id="25ee2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="25ee2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25ee2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ee2-125">Authorization</span></span>|<span data-ttu-id="25ee2-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ee2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25ee2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="25ee2-127">Accept</span></span>|<span data-ttu-id="25ee2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="25ee2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25ee2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25ee2-129">Request body</span></span>
<span data-ttu-id="25ee2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25ee2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ee2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ee2-131">Response</span></span>
<span data-ttu-id="25ee2-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="25ee2-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ee2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="25ee2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="25ee2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="25ee2-134">Request</span></span>
<span data-ttu-id="25ee2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25ee2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="25ee2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ee2-136">Response</span></span>
<span data-ttu-id="25ee2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25ee2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
    "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
    "displayName": "Display Name value",
    "hasRequiredSetting": true
  }
}
```




