---
title: Получение Сиделоадингкэй
description: Чтение свойств и связей объекта Сиделоадингкэй.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e13164ba4288a9e7348778eccf85b9a5e2da56e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983549"
---
# <a name="get-sideloadingkey"></a><span data-ttu-id="575c8-103">Получение Сиделоадингкэй</span><span class="sxs-lookup"><span data-stu-id="575c8-103">Get sideLoadingKey</span></span>

> <span data-ttu-id="575c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="575c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="575c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="575c8-106">Чтение свойств и связей объекта [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="575c8-106">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="575c8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="575c8-107">Prerequisites</span></span>
<span data-ttu-id="575c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="575c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="575c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="575c8-110">Permission type</span></span>|<span data-ttu-id="575c8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="575c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="575c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="575c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="575c8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="575c8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="575c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="575c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="575c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575c8-115">Not supported.</span></span>|
|<span data-ttu-id="575c8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="575c8-116">Application</span></span>|<span data-ttu-id="575c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="575c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="575c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="575c8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="575c8-119">Optional query parameters</span></span>
<span data-ttu-id="575c8-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="575c8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="575c8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="575c8-121">Request headers</span></span>
|<span data-ttu-id="575c8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="575c8-122">Header</span></span>|<span data-ttu-id="575c8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="575c8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="575c8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="575c8-124">Authorization</span></span>|<span data-ttu-id="575c8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="575c8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="575c8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="575c8-126">Accept</span></span>|<span data-ttu-id="575c8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="575c8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="575c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="575c8-128">Request body</span></span>
<span data-ttu-id="575c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="575c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="575c8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="575c8-130">Response</span></span>
<span data-ttu-id="575c8-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="575c8-131">If successful, this method returns a `200 OK` response code and [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="575c8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="575c8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="575c8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="575c8-133">Request</span></span>
<span data-ttu-id="575c8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="575c8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="575c8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="575c8-135">Response</span></span>
<span data-ttu-id="575c8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="575c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




