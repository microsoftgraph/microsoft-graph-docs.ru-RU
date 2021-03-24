---
title: Список встроенныхSIMActivationCodePools
description: Список свойств и связей встроенных объектовSIMActivationCodePool.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd3afc4f45984d6ee525e1dc6cfc84a48e3876b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126152"
---
# <a name="list-embeddedsimactivationcodepools"></a><span data-ttu-id="47f28-103">Список встроенныхSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="47f28-103">List embeddedSIMActivationCodePools</span></span>

<span data-ttu-id="47f28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47f28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47f28-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47f28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f28-107">Список свойств и связей встроенных [объектовSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="47f28-107">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47f28-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47f28-108">Prerequisites</span></span>
<span data-ttu-id="47f28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f28-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f28-111">Permission type</span></span>|<span data-ttu-id="47f28-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47f28-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47f28-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f28-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47f28-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47f28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f28-116">Not supported.</span></span>|
|<span data-ttu-id="47f28-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47f28-117">Application</span></span>|<span data-ttu-id="47f28-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f28-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47f28-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="47f28-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47f28-120">Request headers</span></span>
|<span data-ttu-id="47f28-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47f28-121">Header</span></span>|<span data-ttu-id="47f28-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47f28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47f28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f28-123">Authorization</span></span>|<span data-ttu-id="47f28-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47f28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47f28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47f28-125">Accept</span></span>|<span data-ttu-id="47f28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47f28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47f28-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47f28-127">Request body</span></span>
<span data-ttu-id="47f28-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47f28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f28-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f28-129">Response</span></span>
<span data-ttu-id="47f28-130">В случае успеха этот метод возвращает код отклика и коллекцию встроенных `200 OK` [объектовSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47f28-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f28-131">Пример</span><span class="sxs-lookup"><span data-stu-id="47f28-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="47f28-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f28-132">Request</span></span>
<span data-ttu-id="47f28-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f28-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### <a name="response"></a><span data-ttu-id="47f28-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f28-134">Response</span></span>
<span data-ttu-id="47f28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47f28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 717

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
      "id": "ec308741-8741-ec30-4187-30ec418730ec",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "activationCodes": [
        {
          "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
          "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
          "matchingIdentifier": "Matching Identifier value",
          "smdpPlusServerAddress": "Smdp Plus Server Address value"
        }
      ],
      "activationCodeCount": 3
    }
  ]
}
```




