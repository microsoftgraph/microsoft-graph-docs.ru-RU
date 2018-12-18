---
title: Get termsAndConditionsAcceptanceStatus
description: Чтение свойств и связей объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
ms.openlocfilehash: 6219be740c0dc945e61983d93e39529c48cbc56a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307681"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="1cdbf-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1cdbf-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1cdbf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cdbf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cdbf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cdbf-107">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1cdbf-107">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cdbf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1cdbf-108">Prerequisites</span></span>
<span data-ttu-id="1cdbf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cdbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cdbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cdbf-111">Permission type</span></span>|<span data-ttu-id="1cdbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cdbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cdbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cdbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cdbf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cdbf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1cdbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cdbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cdbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-116">Not supported.</span></span>|
|<span data-ttu-id="1cdbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cdbf-117">Application</span></span>|<span data-ttu-id="1cdbf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cdbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cdbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cdbf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1cdbf-120">Optional query parameters</span></span>
<span data-ttu-id="1cdbf-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1cdbf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cdbf-122">Request headers</span></span>
|<span data-ttu-id="1cdbf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cdbf-123">Header</span></span>|<span data-ttu-id="1cdbf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1cdbf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cdbf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cdbf-125">Authorization</span></span>|<span data-ttu-id="1cdbf-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cdbf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cdbf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1cdbf-127">Accept</span></span>|<span data-ttu-id="1cdbf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1cdbf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cdbf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cdbf-129">Request body</span></span>
<span data-ttu-id="1cdbf-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cdbf-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cdbf-131">Response</span></span>
<span data-ttu-id="1cdbf-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cdbf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1cdbf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cdbf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cdbf-134">Request</span></span>
<span data-ttu-id="1cdbf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="1cdbf-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cdbf-136">Response</span></span>
<span data-ttu-id="1cdbf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cdbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





