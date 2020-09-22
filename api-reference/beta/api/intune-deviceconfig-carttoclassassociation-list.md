---
title: Список свойства carttoclassassociations
description: Список свойств и связей объектов КарттоклассассоЦиатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02e7fe3ea0b3de7b3764dc79ffe0a645a640b829
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072711"
---
# <a name="list-carttoclassassociations"></a><span data-ttu-id="43da7-103">Список свойства carttoclassassociations</span><span class="sxs-lookup"><span data-stu-id="43da7-103">List cartToClassAssociations</span></span>

<span data-ttu-id="43da7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43da7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43da7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43da7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43da7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43da7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43da7-107">Список свойств и связей объектов [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="43da7-107">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43da7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43da7-108">Prerequisites</span></span>
<span data-ttu-id="43da7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43da7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43da7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43da7-111">Permission type</span></span>|<span data-ttu-id="43da7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43da7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43da7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43da7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43da7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43da7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43da7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43da7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43da7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43da7-116">Not supported.</span></span>|
|<span data-ttu-id="43da7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43da7-117">Application</span></span>|<span data-ttu-id="43da7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43da7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43da7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43da7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="43da7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43da7-120">Request headers</span></span>
|<span data-ttu-id="43da7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43da7-121">Header</span></span>|<span data-ttu-id="43da7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43da7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43da7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43da7-123">Authorization</span></span>|<span data-ttu-id="43da7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43da7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43da7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43da7-125">Accept</span></span>|<span data-ttu-id="43da7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43da7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43da7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43da7-127">Request body</span></span>
<span data-ttu-id="43da7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43da7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43da7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="43da7-129">Response</span></span>
<span data-ttu-id="43da7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43da7-130">If successful, this method returns a `200 OK` response code and a collection of [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43da7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="43da7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43da7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="43da7-132">Request</span></span>
<span data-ttu-id="43da7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43da7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
```

### <a name="response"></a><span data-ttu-id="43da7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="43da7-134">Response</span></span>
<span data-ttu-id="43da7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43da7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cartToClassAssociation",
      "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "deviceCartIds": [
        "Device Cart Ids value"
      ],
      "classroomIds": [
        "Classroom Ids value"
      ]
    }
  ]
}
```






