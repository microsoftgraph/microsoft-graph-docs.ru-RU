---
title: Действие assign
description: Замените все целевые группы для политики.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b41ce4ec1c6e304168aebb4c53b4512b0a11f4b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858669"
---
# <a name="assign-action"></a><span data-ttu-id="4b747-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="4b747-103">assign action</span></span>

> <span data-ttu-id="4b747-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b747-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b747-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b747-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b747-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b747-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b747-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="4b747-107">Replace all targeted groups for a policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b747-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b747-108">Prerequisites</span></span>
<span data-ttu-id="4b747-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b747-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b747-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b747-111">Permission type</span></span>|<span data-ttu-id="4b747-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b747-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b747-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b747-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b747-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b747-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b747-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b747-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b747-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b747-116">Not supported.</span></span>|
|<span data-ttu-id="4b747-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b747-117">Application</span></span>|<span data-ttu-id="4b747-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b747-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b747-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b747-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4b747-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b747-120">Request headers</span></span>
|<span data-ttu-id="4b747-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b747-121">Header</span></span>|<span data-ttu-id="4b747-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b747-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b747-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b747-123">Authorization</span></span>|<span data-ttu-id="4b747-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b747-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b747-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b747-125">Accept</span></span>|<span data-ttu-id="4b747-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b747-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b747-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b747-127">Request body</span></span>
<span data-ttu-id="4b747-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b747-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4b747-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4b747-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4b747-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b747-130">Property</span></span>|<span data-ttu-id="4b747-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b747-131">Type</span></span>|<span data-ttu-id="4b747-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b747-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b747-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="4b747-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="4b747-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4b747-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4b747-135">Список назначений настройки office</span><span class="sxs-lookup"><span data-stu-id="4b747-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="4b747-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b747-136">Response</span></span>
<span data-ttu-id="4b747-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b747-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b747-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4b747-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b747-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b747-139">Request</span></span>
<span data-ttu-id="4b747-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b747-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
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

### <a name="response"></a><span data-ttu-id="4b747-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b747-141">Response</span></span>
<span data-ttu-id="4b747-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b747-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



