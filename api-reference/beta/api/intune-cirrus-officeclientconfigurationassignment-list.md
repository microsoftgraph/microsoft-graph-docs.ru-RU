---
title: Список Оффицеклиентконфигуратионассигнментс
description: Список свойств и связей объектов Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: b7b5eeac4c0a07d4cf4e87401a6e0bbf3b11aaf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934014"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="e0f55-103">Список Оффицеклиентконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="e0f55-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="e0f55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0f55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0f55-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0f55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0f55-106">Список свойств и связей объектов [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0f55-106">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0f55-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0f55-107">Prerequisites</span></span>
<span data-ttu-id="e0f55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0f55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0f55-110">Permission type</span></span>|<span data-ttu-id="e0f55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0f55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0f55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0f55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0f55-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="e0f55-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="e0f55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0f55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0f55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0f55-115">Not supported.</span></span>|
|<span data-ttu-id="e0f55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0f55-116">Application</span></span>|<span data-ttu-id="e0f55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0f55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0f55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0f55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e0f55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0f55-119">Request headers</span></span>
|<span data-ttu-id="e0f55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0f55-120">Header</span></span>|<span data-ttu-id="e0f55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0f55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0f55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0f55-122">Authorization</span></span>|<span data-ttu-id="e0f55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0f55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0f55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0f55-124">Accept</span></span>|<span data-ttu-id="e0f55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0f55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0f55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0f55-126">Request body</span></span>
<span data-ttu-id="e0f55-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0f55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0f55-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0f55-128">Response</span></span>
<span data-ttu-id="e0f55-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0f55-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0f55-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e0f55-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0f55-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0f55-131">Request</span></span>
<span data-ttu-id="e0f55-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0f55-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="e0f55-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0f55-133">Response</span></span>
<span data-ttu-id="e0f55-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0f55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



