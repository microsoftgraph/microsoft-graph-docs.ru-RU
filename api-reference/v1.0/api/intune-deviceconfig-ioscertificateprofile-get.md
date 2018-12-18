---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: tfitzmac
ms.openlocfilehash: 9bfdb14f9b7aec9e5446b0c266d4ee59b5e91860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328555"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="959b6-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="959b6-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="959b6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="959b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="959b6-105">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="959b6-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="959b6-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="959b6-106">Prerequisites</span></span>
<span data-ttu-id="959b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="959b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="959b6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="959b6-109">Permission type</span></span>|<span data-ttu-id="959b6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="959b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="959b6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="959b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="959b6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="959b6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="959b6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="959b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="959b6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="959b6-114">Not supported.</span></span>|
|<span data-ttu-id="959b6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="959b6-115">Application</span></span>|<span data-ttu-id="959b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="959b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="959b6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="959b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="959b6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="959b6-118">Optional query parameters</span></span>
<span data-ttu-id="959b6-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="959b6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="959b6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="959b6-120">Request headers</span></span>
|<span data-ttu-id="959b6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="959b6-121">Header</span></span>|<span data-ttu-id="959b6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="959b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="959b6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="959b6-123">Authorization</span></span>|<span data-ttu-id="959b6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="959b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="959b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="959b6-125">Accept</span></span>|<span data-ttu-id="959b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="959b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="959b6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="959b6-127">Request body</span></span>
<span data-ttu-id="959b6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="959b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="959b6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="959b6-129">Response</span></span>
<span data-ttu-id="959b6-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="959b6-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="959b6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="959b6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="959b6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="959b6-132">Request</span></span>
<span data-ttu-id="959b6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="959b6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="959b6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="959b6-134">Response</span></span>
<span data-ttu-id="959b6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="959b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



