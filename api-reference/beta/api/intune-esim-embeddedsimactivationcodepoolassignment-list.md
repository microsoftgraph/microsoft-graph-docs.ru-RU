---
title: Список embeddedSIMActivationCodePoolAssignments
description: Свойства списка и связей объектов embeddedSIMActivationCodePoolAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 885d962771e7fb388269339ac32329114deada6a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404031"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="05805-103">Список embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="05805-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="05805-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05805-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05805-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05805-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05805-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05805-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05805-107">Свойства списка и связей объектов [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="05805-107">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05805-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="05805-108">Prerequisites</span></span>
<span data-ttu-id="05805-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="05805-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05805-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05805-111">Permission type</span></span>|<span data-ttu-id="05805-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05805-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05805-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05805-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05805-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05805-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05805-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05805-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05805-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05805-116">Not supported.</span></span>|
|<span data-ttu-id="05805-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05805-117">Application</span></span>|<span data-ttu-id="05805-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05805-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05805-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05805-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="05805-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05805-120">Request headers</span></span>
|<span data-ttu-id="05805-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05805-121">Header</span></span>|<span data-ttu-id="05805-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05805-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05805-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05805-123">Authorization</span></span>|<span data-ttu-id="05805-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05805-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05805-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05805-125">Accept</span></span>|<span data-ttu-id="05805-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05805-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05805-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05805-127">Request body</span></span>
<span data-ttu-id="05805-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05805-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05805-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="05805-129">Response</span></span>
<span data-ttu-id="05805-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="05805-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05805-131">Пример</span><span class="sxs-lookup"><span data-stu-id="05805-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="05805-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="05805-132">Request</span></span>
<span data-ttu-id="05805-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05805-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="05805-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="05805-134">Response</span></span>
<span data-ttu-id="05805-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05805-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




