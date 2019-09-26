---
title: Список Макманажедапппротектионс
description: Список свойств и связей объектов Макманажедапппротектион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a16d41a3c1916d4d5f81f5e7cf7a3634db9938d9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192700"
---
# <a name="list-macmanagedappprotections"></a><span data-ttu-id="4327a-103">Список Макманажедапппротектионс</span><span class="sxs-lookup"><span data-stu-id="4327a-103">List macManagedAppProtections</span></span>

> <span data-ttu-id="4327a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4327a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4327a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4327a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4327a-106">Список свойств и связей объектов [макманажедапппротектион](../resources/intune-policyset-macmanagedappprotection.md) .</span><span class="sxs-lookup"><span data-stu-id="4327a-106">List properties and relationships of the [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4327a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4327a-107">Prerequisites</span></span>
<span data-ttu-id="4327a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4327a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4327a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4327a-110">Permission type</span></span>|<span data-ttu-id="4327a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4327a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4327a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4327a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4327a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4327a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4327a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4327a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4327a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4327a-115">Not supported.</span></span>|
|<span data-ttu-id="4327a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4327a-116">Application</span></span>|<span data-ttu-id="4327a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4327a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4327a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4327a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/macManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="4327a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4327a-119">Request headers</span></span>
|<span data-ttu-id="4327a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4327a-120">Header</span></span>|<span data-ttu-id="4327a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4327a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4327a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4327a-122">Authorization</span></span>|<span data-ttu-id="4327a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4327a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4327a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4327a-124">Accept</span></span>|<span data-ttu-id="4327a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4327a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4327a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4327a-126">Request body</span></span>
<span data-ttu-id="4327a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4327a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4327a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4327a-128">Response</span></span>
<span data-ttu-id="4327a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макманажедапппротектион](../resources/intune-policyset-macmanagedappprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4327a-129">If successful, this method returns a `200 OK` response code and a collection of [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4327a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4327a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4327a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4327a-131">Request</span></span>
<span data-ttu-id="4327a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4327a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/macManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="4327a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4327a-133">Response</span></span>
<span data-ttu-id="4327a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4327a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macManagedAppProtection",
      "id": "bb139531-9531-bb13-3195-13bb319513bb"
    }
  ]
}
```




