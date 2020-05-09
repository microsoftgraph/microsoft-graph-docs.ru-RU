---
title: Список Ембеддедсимактиватионкодепулассигнментс
description: Список свойств и связей объектов Ембеддедсимактиватионкодепулассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecd136e8be61b2c4ca2666b95bf61a88beff9144
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44174610"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="46ec5-103">Список Ембеддедсимактиватионкодепулассигнментс</span><span class="sxs-lookup"><span data-stu-id="46ec5-103">List embeddedSIMActivationCodePoolAssignments</span></span>

<span data-ttu-id="46ec5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46ec5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46ec5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ec5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46ec5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46ec5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ec5-107">Список свойств и связей объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="46ec5-107">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46ec5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46ec5-108">Prerequisites</span></span>
<span data-ttu-id="46ec5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ec5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ec5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ec5-111">Permission type</span></span>|<span data-ttu-id="46ec5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ec5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46ec5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ec5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46ec5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46ec5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="46ec5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ec5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ec5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ec5-116">Not supported.</span></span>|
|<span data-ttu-id="46ec5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46ec5-117">Application</span></span>|<span data-ttu-id="46ec5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46ec5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46ec5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ec5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="46ec5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46ec5-120">Request headers</span></span>
|<span data-ttu-id="46ec5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46ec5-121">Header</span></span>|<span data-ttu-id="46ec5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46ec5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46ec5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46ec5-123">Authorization</span></span>|<span data-ttu-id="46ec5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46ec5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46ec5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46ec5-125">Accept</span></span>|<span data-ttu-id="46ec5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46ec5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46ec5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46ec5-127">Request body</span></span>
<span data-ttu-id="46ec5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46ec5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46ec5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="46ec5-129">Response</span></span>
<span data-ttu-id="46ec5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46ec5-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46ec5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="46ec5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="46ec5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ec5-132">Request</span></span>
<span data-ttu-id="46ec5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ec5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="46ec5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ec5-134">Response</span></span>
<span data-ttu-id="46ec5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46ec5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      }
    }
  ]
}
```



