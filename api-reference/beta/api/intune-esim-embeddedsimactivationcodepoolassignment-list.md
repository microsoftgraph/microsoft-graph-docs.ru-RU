---
title: Список Ембеддедсимактиватионкодепулассигнментс
description: Список свойств и связей объектов Ембеддедсимактиватионкодепулассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 930513219b54e5e0a1de10bcfd85ab16ce6c193b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173523"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="258d5-103">Список Ембеддедсимактиватионкодепулассигнментс</span><span class="sxs-lookup"><span data-stu-id="258d5-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="258d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="258d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="258d5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="258d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="258d5-106">Список свойств и связей объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="258d5-106">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="258d5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="258d5-107">Prerequisites</span></span>
<span data-ttu-id="258d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="258d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="258d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="258d5-110">Permission type</span></span>|<span data-ttu-id="258d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="258d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="258d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="258d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="258d5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="258d5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="258d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="258d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="258d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="258d5-115">Not supported.</span></span>|
|<span data-ttu-id="258d5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="258d5-116">Application</span></span>|<span data-ttu-id="258d5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="258d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="258d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="258d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="258d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="258d5-119">Request headers</span></span>
|<span data-ttu-id="258d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="258d5-120">Header</span></span>|<span data-ttu-id="258d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="258d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="258d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="258d5-122">Authorization</span></span>|<span data-ttu-id="258d5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="258d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="258d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="258d5-124">Accept</span></span>|<span data-ttu-id="258d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="258d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="258d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="258d5-126">Request body</span></span>
<span data-ttu-id="258d5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="258d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="258d5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="258d5-128">Response</span></span>
<span data-ttu-id="258d5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="258d5-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="258d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="258d5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="258d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="258d5-131">Request</span></span>
<span data-ttu-id="258d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="258d5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="258d5-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="258d5-133">Response</span></span>
<span data-ttu-id="258d5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="258d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




