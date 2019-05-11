---
title: Получение Девицеманажементколлектионсеттингинстанце
description: Чтение свойств и связей объекта Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b314ee41522288b6297a8ad66a1573bf38899f6a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916737"
---
# <a name="get-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="17acc-103">Получение Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="17acc-103">Get deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="17acc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17acc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17acc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17acc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17acc-106">Чтение свойств и связей объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="17acc-106">Read properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17acc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17acc-107">Prerequisites</span></span>
<span data-ttu-id="17acc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17acc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17acc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17acc-110">Permission type</span></span>|<span data-ttu-id="17acc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17acc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17acc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17acc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17acc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17acc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17acc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17acc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17acc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17acc-115">Not supported.</span></span>|
|<span data-ttu-id="17acc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17acc-116">Application</span></span>|<span data-ttu-id="17acc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17acc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17acc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17acc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17acc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17acc-119">Optional query parameters</span></span>
<span data-ttu-id="17acc-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17acc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17acc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17acc-121">Request headers</span></span>
|<span data-ttu-id="17acc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17acc-122">Header</span></span>|<span data-ttu-id="17acc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="17acc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17acc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17acc-124">Authorization</span></span>|<span data-ttu-id="17acc-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17acc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17acc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="17acc-126">Accept</span></span>|<span data-ttu-id="17acc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17acc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17acc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17acc-128">Request body</span></span>
<span data-ttu-id="17acc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17acc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17acc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="17acc-130">Response</span></span>
<span data-ttu-id="17acc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17acc-131">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17acc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="17acc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17acc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="17acc-133">Request</span></span>
<span data-ttu-id="17acc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17acc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="17acc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="17acc-135">Response</span></span>
<span data-ttu-id="17acc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17acc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
    "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value"
  }
}
```




