---
title: Список officeClientConfigurationAssignments
description: Список свойств и связей объектов officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 570281f3961f1f4449ae9050cd77b12863452fc3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665924"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="de7d1-103">Список officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="de7d1-103">List officeClientConfigurationAssignments</span></span>

<span data-ttu-id="de7d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de7d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de7d1-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de7d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de7d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de7d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de7d1-107">Список свойств и связей [объектов officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de7d1-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de7d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de7d1-108">Prerequisites</span></span>
<span data-ttu-id="de7d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de7d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de7d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de7d1-111">Permission type</span></span>|<span data-ttu-id="de7d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de7d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de7d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de7d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de7d1-114">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="de7d1-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="de7d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de7d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de7d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de7d1-116">Not supported.</span></span>|
|<span data-ttu-id="de7d1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de7d1-117">Application</span></span>|<span data-ttu-id="de7d1-118">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="de7d1-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="de7d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de7d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="de7d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de7d1-120">Request headers</span></span>
|<span data-ttu-id="de7d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de7d1-121">Header</span></span>|<span data-ttu-id="de7d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de7d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de7d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de7d1-123">Authorization</span></span>|<span data-ttu-id="de7d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de7d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de7d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de7d1-125">Accept</span></span>|<span data-ttu-id="de7d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de7d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de7d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de7d1-127">Request body</span></span>
<span data-ttu-id="de7d1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de7d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de7d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="de7d1-129">Response</span></span>
<span data-ttu-id="de7d1-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию `200 OK` [объектов officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de7d1-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de7d1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="de7d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="de7d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="de7d1-132">Request</span></span>
<span data-ttu-id="de7d1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de7d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="de7d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="de7d1-134">Response</span></span>
<span data-ttu-id="de7d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de7d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




