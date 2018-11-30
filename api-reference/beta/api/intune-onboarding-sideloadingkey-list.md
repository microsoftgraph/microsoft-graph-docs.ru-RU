---
title: Список sideLoadingKeies
description: Свойства списка и связей объектов sideLoadingKey.
ms.openlocfilehash: 423279fe3a82655e0cc338043070a9e7033151a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082792"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="9ab96-103">Список sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="9ab96-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="9ab96-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ab96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ab96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ab96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9ab96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ab96-107">Свойства списка и связей объектов [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="9ab96-107">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ab96-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9ab96-108">Prerequisites</span></span>
<span data-ttu-id="9ab96-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab96-111">Permission type</span></span>|<span data-ttu-id="9ab96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ab96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ab96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab96-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ab96-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9ab96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ab96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab96-116">Not supported.</span></span>|
|<span data-ttu-id="9ab96-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ab96-117">Application</span></span>|<span data-ttu-id="9ab96-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="9ab96-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ab96-120">Request headers</span></span>
|<span data-ttu-id="9ab96-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ab96-121">Header</span></span>|<span data-ttu-id="9ab96-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ab96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ab96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ab96-123">Authorization</span></span>|<span data-ttu-id="9ab96-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9ab96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ab96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ab96-125">Accept</span></span>|<span data-ttu-id="9ab96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab96-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ab96-127">Request body</span></span>
<span data-ttu-id="9ab96-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ab96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab96-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ab96-129">Response</span></span>
<span data-ttu-id="9ab96-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9ab96-130">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9ab96-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ab96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab96-132">Request</span></span>
<span data-ttu-id="9ab96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ab96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="9ab96-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ab96-134">Response</span></span>
<span data-ttu-id="9ab96-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9ab96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```





