---
title: Get termsAndConditionsAcceptanceStatus
description: Чтение свойств и связей объекта termsAndConditionsAcceptanceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd5f5bd201d4b008e4ad0d0bad7e65e724394eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418290"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="a9def-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="a9def-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="a9def-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9def-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9def-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9def-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9def-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9def-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9def-107">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a9def-107">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9def-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a9def-108">Prerequisites</span></span>
<span data-ttu-id="a9def-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9def-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9def-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9def-111">Permission type</span></span>|<span data-ttu-id="a9def-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9def-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9def-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9def-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9def-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9def-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a9def-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9def-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9def-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9def-116">Not supported.</span></span>|
|<span data-ttu-id="a9def-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9def-117">Application</span></span>|<span data-ttu-id="a9def-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9def-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9def-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9def-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9def-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9def-120">Optional query parameters</span></span>
<span data-ttu-id="a9def-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a9def-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9def-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9def-122">Request headers</span></span>
|<span data-ttu-id="a9def-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9def-123">Header</span></span>|<span data-ttu-id="a9def-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a9def-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9def-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9def-125">Authorization</span></span>|<span data-ttu-id="a9def-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a9def-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9def-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a9def-127">Accept</span></span>|<span data-ttu-id="a9def-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a9def-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9def-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9def-129">Request body</span></span>
<span data-ttu-id="a9def-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9def-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9def-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9def-131">Response</span></span>
<span data-ttu-id="a9def-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a9def-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9def-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a9def-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9def-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9def-134">Request</span></span>
<span data-ttu-id="a9def-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9def-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="a9def-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9def-136">Response</span></span>
<span data-ttu-id="a9def-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9def-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




