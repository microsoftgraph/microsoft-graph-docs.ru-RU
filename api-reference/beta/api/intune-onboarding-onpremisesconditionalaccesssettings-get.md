---
title: Получение объекта onPremisesConditionalAccessSettings
description: Чтение свойств и связей объекта onPremisesConditionalAccessSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6de2ae6866018ffb8411bf3ce0cb2999f320474e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190441"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="7e64c-103">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="7e64c-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="7e64c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e64c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e64c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e64c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e64c-106">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="7e64c-106">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e64c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e64c-107">Prerequisites</span></span>
<span data-ttu-id="7e64c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e64c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e64c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e64c-110">Permission type</span></span>|<span data-ttu-id="7e64c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e64c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e64c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e64c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e64c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e64c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7e64c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e64c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e64c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e64c-115">Not supported.</span></span>|
|<span data-ttu-id="7e64c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e64c-116">Application</span></span>|<span data-ttu-id="7e64c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e64c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e64c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e64c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e64c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e64c-119">Optional query parameters</span></span>
<span data-ttu-id="7e64c-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e64c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e64c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e64c-121">Request headers</span></span>
|<span data-ttu-id="7e64c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e64c-122">Header</span></span>|<span data-ttu-id="7e64c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e64c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e64c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e64c-124">Authorization</span></span>|<span data-ttu-id="7e64c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e64c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e64c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7e64c-126">Accept</span></span>|<span data-ttu-id="7e64c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e64c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e64c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e64c-128">Request body</span></span>
<span data-ttu-id="7e64c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e64c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e64c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e64c-130">Response</span></span>
<span data-ttu-id="7e64c-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e64c-131">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e64c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7e64c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e64c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e64c-133">Request</span></span>
<span data-ttu-id="7e64c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e64c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="7e64c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e64c-135">Response</span></span>
<span data-ttu-id="7e64c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e64c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```




