---
title: Получение sideLoadingKey
description: Чтение свойства и связи объекта sideLoadingKey.
author: tfitzmac
ms.openlocfilehash: cae8f35c31072cf7078a50eae4a9691bd9516f8b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308647"
---
# <a name="get-sideloadingkey"></a><span data-ttu-id="e6a40-103">Получение sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="e6a40-103">Get sideLoadingKey</span></span>

> <span data-ttu-id="e6a40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6a40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6a40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6a40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e6a40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6a40-107">Чтение свойства и связи объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="e6a40-107">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6a40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6a40-108">Prerequisites</span></span>
<span data-ttu-id="e6a40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a40-111">Permission type</span></span>|<span data-ttu-id="e6a40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6a40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6a40-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6a40-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e6a40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6a40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a40-116">Not supported.</span></span>|
|<span data-ttu-id="e6a40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6a40-117">Application</span></span>|<span data-ttu-id="e6a40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6a40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6a40-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6a40-120">Optional query parameters</span></span>
<span data-ttu-id="e6a40-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6a40-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e6a40-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6a40-122">Request headers</span></span>
|<span data-ttu-id="e6a40-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6a40-123">Header</span></span>|<span data-ttu-id="e6a40-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e6a40-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6a40-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6a40-125">Authorization</span></span>|<span data-ttu-id="e6a40-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6a40-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6a40-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e6a40-127">Accept</span></span>|<span data-ttu-id="e6a40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e6a40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a40-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6a40-129">Request body</span></span>
<span data-ttu-id="e6a40-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6a40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a40-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6a40-131">Response</span></span>
<span data-ttu-id="e6a40-132">Успешно завершена, этот метод возвращает `200 OK` объект [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6a40-132">If successful, this method returns a `200 OK` response code and [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a40-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e6a40-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6a40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6a40-134">Request</span></span>
<span data-ttu-id="e6a40-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6a40-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="e6a40-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6a40-136">Response</span></span>
<span data-ttu-id="e6a40-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e6a40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





