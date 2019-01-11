---
title: Обновление officeClientConfigurationAssignment
description: Обновление свойства объекта officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f3d2fab5dc8793f566973e2d3e2d9bf968cbf30a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817530"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="433b6-103">Обновление officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="433b6-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="433b6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="433b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="433b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="433b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="433b6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="433b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="433b6-107">Обновление свойства объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="433b6-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="433b6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="433b6-108">Prerequisites</span></span>
<span data-ttu-id="433b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="433b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="433b6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="433b6-111">Permission type</span></span>|<span data-ttu-id="433b6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="433b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="433b6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="433b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="433b6-114">\*\* ЗАДАЧ: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="433b6-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="433b6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="433b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="433b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="433b6-116">Not supported.</span></span>|
|<span data-ttu-id="433b6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="433b6-117">Application</span></span>|<span data-ttu-id="433b6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="433b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="433b6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="433b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="433b6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="433b6-120">Request headers</span></span>
|<span data-ttu-id="433b6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="433b6-121">Header</span></span>|<span data-ttu-id="433b6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="433b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="433b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="433b6-123">Authorization</span></span>|<span data-ttu-id="433b6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="433b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="433b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="433b6-125">Accept</span></span>|<span data-ttu-id="433b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="433b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="433b6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="433b6-127">Request body</span></span>
<span data-ttu-id="433b6-128">В тексте запроса укажите представление JSON для объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="433b6-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="433b6-129">В следующей таблице показаны свойства, которые необходимы для создания [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="433b6-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="433b6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="433b6-130">Property</span></span>|<span data-ttu-id="433b6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="433b6-131">Type</span></span>|<span data-ttu-id="433b6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="433b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="433b6-133">id</span><span class="sxs-lookup"><span data-stu-id="433b6-133">id</span></span>|<span data-ttu-id="433b6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="433b6-134">String</span></span>|<span data-ttu-id="433b6-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="433b6-135">Not yet documented</span></span>|
|<span data-ttu-id="433b6-136">target</span><span class="sxs-lookup"><span data-stu-id="433b6-136">target</span></span>|[<span data-ttu-id="433b6-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="433b6-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="433b6-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="433b6-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="433b6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="433b6-139">Response</span></span>
<span data-ttu-id="433b6-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="433b6-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="433b6-141">Пример</span><span class="sxs-lookup"><span data-stu-id="433b6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="433b6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="433b6-142">Request</span></span>
<span data-ttu-id="433b6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="433b6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="433b6-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="433b6-144">Response</span></span>
<span data-ttu-id="433b6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="433b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



