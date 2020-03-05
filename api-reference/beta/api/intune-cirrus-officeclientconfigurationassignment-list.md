---
title: Список Оффицеклиентконфигуратионассигнментс
description: Список свойств и связей объектов Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1558d9aa0360855d6f6c8ce03ff4c74786e04c14
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444429"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="2608a-103">Список Оффицеклиентконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="2608a-103">List officeClientConfigurationAssignments</span></span>

<span data-ttu-id="2608a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2608a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2608a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2608a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2608a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2608a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2608a-107">Список свойств и связей объектов [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2608a-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2608a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2608a-108">Prerequisites</span></span>
<span data-ttu-id="2608a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2608a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2608a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2608a-111">Permission type</span></span>|<span data-ttu-id="2608a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2608a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2608a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2608a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2608a-114">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="2608a-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="2608a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2608a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2608a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2608a-116">Not supported.</span></span>|
|<span data-ttu-id="2608a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2608a-117">Application</span></span>|<span data-ttu-id="2608a-118">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="2608a-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="2608a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2608a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2608a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2608a-120">Request headers</span></span>
|<span data-ttu-id="2608a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2608a-121">Header</span></span>|<span data-ttu-id="2608a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2608a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2608a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2608a-123">Authorization</span></span>|<span data-ttu-id="2608a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2608a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2608a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2608a-125">Accept</span></span>|<span data-ttu-id="2608a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2608a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2608a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2608a-127">Request body</span></span>
<span data-ttu-id="2608a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2608a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2608a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2608a-129">Response</span></span>
<span data-ttu-id="2608a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2608a-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2608a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2608a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2608a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2608a-132">Request</span></span>
<span data-ttu-id="2608a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2608a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="2608a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2608a-134">Response</span></span>
<span data-ttu-id="2608a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2608a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





