---
title: Получение Сиделоадингкэй
description: Чтение свойств и связей объекта Сиделоадингкэй.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f048c33de07d07321295d7771ef1bafb9e618376
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801773"
---
# <a name="get-sideloadingkey"></a><span data-ttu-id="e2832-103">Получение Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="e2832-103">Get sideLoadingKey</span></span>

> <span data-ttu-id="e2832-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2832-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2832-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2832-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2832-106">Чтение свойств и связей объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="e2832-106">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2832-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2832-107">Prerequisites</span></span>
<span data-ttu-id="e2832-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2832-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2832-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2832-110">Permission type</span></span>|<span data-ttu-id="e2832-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2832-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2832-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2832-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2832-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2832-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e2832-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2832-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2832-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2832-115">Not supported.</span></span>|
|<span data-ttu-id="e2832-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2832-116">Application</span></span>|<span data-ttu-id="e2832-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2832-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2832-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2832-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2832-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2832-119">Optional query parameters</span></span>
<span data-ttu-id="e2832-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2832-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2832-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2832-121">Request headers</span></span>
|<span data-ttu-id="e2832-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2832-122">Header</span></span>|<span data-ttu-id="e2832-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e2832-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2832-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2832-124">Authorization</span></span>|<span data-ttu-id="e2832-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2832-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2832-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e2832-126">Accept</span></span>|<span data-ttu-id="e2832-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2832-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2832-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2832-128">Request body</span></span>
<span data-ttu-id="e2832-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2832-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2832-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2832-130">Response</span></span>
<span data-ttu-id="e2832-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2832-131">If successful, this method returns a `200 OK` response code and [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2832-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e2832-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2832-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2832-133">Request</span></span>
<span data-ttu-id="e2832-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2832-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="e2832-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2832-135">Response</span></span>
<span data-ttu-id="e2832-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2832-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "value": {
    "@odata.type": "#microsoft.graph.sideLoadingKey",
    "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
    "value": "Value value",
    "displayName": "Display Name value",
    "description": "Description value",
    "totalActivation": 15,
    "lastUpdatedDateTime": "Last Updated Date Time value"
  }
}
```





