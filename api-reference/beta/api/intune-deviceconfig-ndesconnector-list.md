---
title: Список ndesConnectors
description: Свойства списка и связей объектов ndesConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 52da3f3cf0936a13cc210c4be4092d24dd5b6317
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402414"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="ee89b-103">Список ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="ee89b-103">List ndesConnectors</span></span>

> <span data-ttu-id="ee89b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee89b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee89b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee89b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee89b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee89b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee89b-107">Свойства списка и связей объектов [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="ee89b-107">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee89b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ee89b-108">Prerequisites</span></span>
<span data-ttu-id="ee89b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee89b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee89b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee89b-111">Permission type</span></span>|<span data-ttu-id="ee89b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee89b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee89b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee89b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee89b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee89b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ee89b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee89b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee89b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee89b-116">Not supported.</span></span>|
|<span data-ttu-id="ee89b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee89b-117">Application</span></span>|<span data-ttu-id="ee89b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee89b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee89b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee89b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ee89b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee89b-120">Request headers</span></span>
|<span data-ttu-id="ee89b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee89b-121">Header</span></span>|<span data-ttu-id="ee89b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee89b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee89b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee89b-123">Authorization</span></span>|<span data-ttu-id="ee89b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee89b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee89b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee89b-125">Accept</span></span>|<span data-ttu-id="ee89b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee89b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee89b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee89b-127">Request body</span></span>
<span data-ttu-id="ee89b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee89b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee89b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee89b-129">Response</span></span>
<span data-ttu-id="ee89b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee89b-130">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee89b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee89b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee89b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee89b-132">Request</span></span>
<span data-ttu-id="ee89b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee89b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="ee89b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee89b-134">Response</span></span>
<span data-ttu-id="ee89b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee89b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```




