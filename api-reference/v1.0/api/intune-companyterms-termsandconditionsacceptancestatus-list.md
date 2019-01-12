---
title: Перечисление объектов termsAndConditionsAcceptanceStatus
description: Список свойств и связей объектов termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8465e4c39d0a7af61e13ce45a107afb69e4a6473
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911751"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="42f3f-103">Перечисление объектов termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="42f3f-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="42f3f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="42f3f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42f3f-105">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="42f3f-105">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42f3f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="42f3f-106">Prerequisites</span></span>
<span data-ttu-id="42f3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42f3f-109">Permission type</span></span>|<span data-ttu-id="42f3f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42f3f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42f3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42f3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42f3f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="42f3f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="42f3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42f3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42f3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f3f-114">Not supported.</span></span>|
|<span data-ttu-id="42f3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42f3f-115">Application</span></span>|<span data-ttu-id="42f3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f3f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42f3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42f3f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="42f3f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42f3f-118">Request headers</span></span>
|<span data-ttu-id="42f3f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42f3f-119">Header</span></span>|<span data-ttu-id="42f3f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="42f3f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42f3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f3f-121">Authorization</span></span>|<span data-ttu-id="42f3f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42f3f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42f3f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="42f3f-123">Accept</span></span>|<span data-ttu-id="42f3f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="42f3f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42f3f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42f3f-125">Request body</span></span>
<span data-ttu-id="42f3f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42f3f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42f3f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="42f3f-127">Response</span></span>
<span data-ttu-id="42f3f-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42f3f-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f3f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="42f3f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="42f3f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="42f3f-130">Request</span></span>
<span data-ttu-id="42f3f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42f3f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="42f3f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="42f3f-132">Response</span></span>
<span data-ttu-id="42f3f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42f3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```



