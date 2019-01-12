---
title: Действие assign
description: Замените все целевые группы для политики.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dc9a3fb0ed7b941d8ebc8d37c9a69e605f0804b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964006"
---
# <a name="assign-action"></a><span data-ttu-id="32327-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="32327-103">assign action</span></span>

> <span data-ttu-id="32327-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32327-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32327-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32327-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32327-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32327-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="32327-107">Replace all targeted groups for a policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32327-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32327-108">Prerequisites</span></span>
<span data-ttu-id="32327-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32327-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32327-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32327-111">Permission type</span></span>|<span data-ttu-id="32327-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32327-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32327-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32327-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32327-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32327-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32327-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32327-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32327-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32327-116">Not supported.</span></span>|
|<span data-ttu-id="32327-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32327-117">Application</span></span>|<span data-ttu-id="32327-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32327-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32327-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32327-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="32327-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32327-120">Request headers</span></span>
|<span data-ttu-id="32327-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32327-121">Header</span></span>|<span data-ttu-id="32327-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32327-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32327-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32327-123">Authorization</span></span>|<span data-ttu-id="32327-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="32327-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32327-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32327-125">Accept</span></span>|<span data-ttu-id="32327-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32327-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32327-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32327-127">Request body</span></span>
<span data-ttu-id="32327-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32327-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32327-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="32327-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32327-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32327-130">Property</span></span>|<span data-ttu-id="32327-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32327-131">Type</span></span>|<span data-ttu-id="32327-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32327-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32327-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="32327-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="32327-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="32327-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="32327-135">Список назначений настройки office</span><span class="sxs-lookup"><span data-stu-id="32327-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="32327-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="32327-136">Response</span></span>
<span data-ttu-id="32327-137">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="32327-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32327-138">Пример</span><span class="sxs-lookup"><span data-stu-id="32327-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="32327-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="32327-139">Request</span></span>
<span data-ttu-id="32327-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32327-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32327-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="32327-141">Response</span></span>
<span data-ttu-id="32327-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="32327-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



