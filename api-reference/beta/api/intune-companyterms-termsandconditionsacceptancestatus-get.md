---
title: Get termsAndConditionsAcceptanceStatus
description: Чтение свойств и связей объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a885af0059006d54a4969ba11c78eb9da94cd007
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32482573"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="dfbdd-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="dfbdd-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="dfbdd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfbdd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfbdd-106">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dfbdd-106">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfbdd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbdd-107">Prerequisites</span></span>
<span data-ttu-id="dfbdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbdd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbdd-110">Permission type</span></span>|<span data-ttu-id="dfbdd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfbdd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfbdd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfbdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfbdd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfbdd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dfbdd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfbdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfbdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-115">Not supported.</span></span>|
|<span data-ttu-id="dfbdd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfbdd-116">Application</span></span>|<span data-ttu-id="dfbdd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfbdd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfbdd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfbdd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfbdd-119">Optional query parameters</span></span>
<span data-ttu-id="dfbdd-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfbdd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfbdd-121">Request headers</span></span>
|<span data-ttu-id="dfbdd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfbdd-122">Header</span></span>|<span data-ttu-id="dfbdd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dfbdd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfbdd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfbdd-124">Authorization</span></span>|<span data-ttu-id="dfbdd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfbdd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dfbdd-126">Accept</span></span>|<span data-ttu-id="dfbdd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dfbdd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfbdd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfbdd-128">Request body</span></span>
<span data-ttu-id="dfbdd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfbdd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfbdd-130">Response</span></span>
<span data-ttu-id="dfbdd-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbdd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dfbdd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfbdd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfbdd-133">Request</span></span>
<span data-ttu-id="dfbdd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="dfbdd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfbdd-135">Response</span></span>
<span data-ttu-id="dfbdd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfbdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```





