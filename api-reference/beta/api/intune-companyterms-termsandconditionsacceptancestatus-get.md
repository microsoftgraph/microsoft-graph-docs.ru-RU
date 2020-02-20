---
title: Get termsAndConditionsAcceptanceStatus
description: Чтение свойств и связей объекта termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 262b1a0006c01ac2613a5322d162855497873df0
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159446"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="7e5f7-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="7e5f7-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="7e5f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e5f7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e5f7-106">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7e5f7-106">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e5f7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7e5f7-107">Prerequisites</span></span>
<span data-ttu-id="7e5f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e5f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e5f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e5f7-110">Permission type</span></span>|<span data-ttu-id="7e5f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e5f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e5f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e5f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e5f7-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e5f7-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7e5f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e5f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e5f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-115">Not supported.</span></span>|
|<span data-ttu-id="7e5f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e5f7-116">Application</span></span>|<span data-ttu-id="7e5f7-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e5f7-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e5f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e5f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e5f7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e5f7-119">Optional query parameters</span></span>
<span data-ttu-id="7e5f7-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e5f7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e5f7-121">Request headers</span></span>
|<span data-ttu-id="7e5f7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e5f7-122">Header</span></span>|<span data-ttu-id="7e5f7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e5f7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e5f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e5f7-124">Authorization</span></span>|<span data-ttu-id="7e5f7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e5f7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7e5f7-126">Accept</span></span>|<span data-ttu-id="7e5f7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e5f7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e5f7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e5f7-128">Request body</span></span>
<span data-ttu-id="7e5f7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e5f7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e5f7-130">Response</span></span>
<span data-ttu-id="7e5f7-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e5f7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7e5f7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e5f7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e5f7-133">Request</span></span>
<span data-ttu-id="7e5f7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="7e5f7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e5f7-135">Response</span></span>
<span data-ttu-id="7e5f7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e5f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





