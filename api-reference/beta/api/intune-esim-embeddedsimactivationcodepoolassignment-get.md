---
title: Получение Ембеддедсимактиватионкодепулассигнмент
description: Чтение свойств и связей объекта Ембеддедсимактиватионкодепулассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94e8a666ba39ea542a824a6f8ebf92a2de427493
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778546"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="61b24-103">Получение Ембеддедсимактиватионкодепулассигнмент</span><span class="sxs-lookup"><span data-stu-id="61b24-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="61b24-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61b24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61b24-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61b24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b24-106">Чтение свойств и связей объекта [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="61b24-106">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61b24-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="61b24-107">Prerequisites</span></span>
<span data-ttu-id="61b24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61b24-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61b24-110">Permission type</span></span>|<span data-ttu-id="61b24-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61b24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61b24-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61b24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61b24-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="61b24-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="61b24-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61b24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61b24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61b24-115">Not supported.</span></span>|
|<span data-ttu-id="61b24-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61b24-116">Application</span></span>|<span data-ttu-id="61b24-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61b24-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61b24-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61b24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61b24-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61b24-119">Optional query parameters</span></span>
<span data-ttu-id="61b24-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61b24-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61b24-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61b24-121">Request headers</span></span>
|<span data-ttu-id="61b24-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61b24-122">Header</span></span>|<span data-ttu-id="61b24-123">Значение</span><span class="sxs-lookup"><span data-stu-id="61b24-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61b24-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61b24-124">Authorization</span></span>|<span data-ttu-id="61b24-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61b24-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61b24-126">Accept</span><span class="sxs-lookup"><span data-stu-id="61b24-126">Accept</span></span>|<span data-ttu-id="61b24-127">application/json</span><span class="sxs-lookup"><span data-stu-id="61b24-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61b24-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61b24-128">Request body</span></span>
<span data-ttu-id="61b24-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61b24-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61b24-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="61b24-130">Response</span></span>
<span data-ttu-id="61b24-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="61b24-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61b24-132">Пример</span><span class="sxs-lookup"><span data-stu-id="61b24-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="61b24-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="61b24-133">Request</span></span>
<span data-ttu-id="61b24-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61b24-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="61b24-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="61b24-135">Response</span></span>
<span data-ttu-id="61b24-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61b24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
    "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





