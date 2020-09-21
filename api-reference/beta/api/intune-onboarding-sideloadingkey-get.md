---
title: Получение Сиделоадингкэй
description: Чтение свойств и связей объекта Сиделоадингкэй.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca20f948afb3ab944664a1cda88910ff9f00740a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043131"
---
# <a name="get-sideloadingkey"></a><span data-ttu-id="85dab-103">Получение Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="85dab-103">Get sideLoadingKey</span></span>

<span data-ttu-id="85dab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85dab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85dab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85dab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85dab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85dab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85dab-107">Чтение свойств и связей объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="85dab-107">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85dab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85dab-108">Prerequisites</span></span>
<span data-ttu-id="85dab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85dab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85dab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85dab-111">Permission type</span></span>|<span data-ttu-id="85dab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85dab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85dab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85dab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85dab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85dab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="85dab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85dab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85dab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85dab-116">Not supported.</span></span>|
|<span data-ttu-id="85dab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85dab-117">Application</span></span>|<span data-ttu-id="85dab-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85dab-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85dab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85dab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85dab-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85dab-120">Optional query parameters</span></span>
<span data-ttu-id="85dab-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85dab-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85dab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85dab-122">Request headers</span></span>
|<span data-ttu-id="85dab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85dab-123">Header</span></span>|<span data-ttu-id="85dab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="85dab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85dab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85dab-125">Authorization</span></span>|<span data-ttu-id="85dab-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85dab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85dab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="85dab-127">Accept</span></span>|<span data-ttu-id="85dab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="85dab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85dab-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85dab-129">Request body</span></span>
<span data-ttu-id="85dab-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85dab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85dab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85dab-131">Response</span></span>
<span data-ttu-id="85dab-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85dab-132">If successful, this method returns a `200 OK` response code and [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85dab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="85dab-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="85dab-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="85dab-134">Request</span></span>
<span data-ttu-id="85dab-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85dab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="85dab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="85dab-136">Response</span></span>
<span data-ttu-id="85dab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85dab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






