---
title: Перечисление объектов iosCertificateProfile
description: Список свойств и связей объектов iosCertificateProfile.
ms.openlocfilehash: 8d683340014892f5154fdda5a614d4de55205747
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026942"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="0019e-103">Перечисление объектов iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0019e-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="0019e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0019e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0019e-105">Список свойств и связей объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0019e-105">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0019e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0019e-106">Prerequisites</span></span>
<span data-ttu-id="0019e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0019e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0019e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0019e-109">Permission type</span></span>|<span data-ttu-id="0019e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0019e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0019e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0019e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0019e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0019e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0019e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0019e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0019e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0019e-114">Not supported.</span></span>|
|<span data-ttu-id="0019e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0019e-115">Application</span></span>|<span data-ttu-id="0019e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0019e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0019e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0019e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0019e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0019e-118">Request headers</span></span>
|<span data-ttu-id="0019e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0019e-119">Header</span></span>|<span data-ttu-id="0019e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0019e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0019e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0019e-121">Authorization</span></span>|<span data-ttu-id="0019e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0019e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0019e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0019e-123">Accept</span></span>|<span data-ttu-id="0019e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0019e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0019e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0019e-125">Request body</span></span>
<span data-ttu-id="0019e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0019e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0019e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0019e-127">Response</span></span>
<span data-ttu-id="0019e-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0019e-128">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0019e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0019e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0019e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0019e-130">Request</span></span>
<span data-ttu-id="0019e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0019e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0019e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0019e-132">Response</span></span>
<span data-ttu-id="0019e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0019e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



