---
title: Обновление Оффицеклиентконфигуратионассигнмент
description: Обновление свойств объекта Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1125ab17915aaf56f5c5a334bd1775c1acf5be8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436752"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="2400f-103">Обновление Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="2400f-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="2400f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2400f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2400f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2400f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2400f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2400f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2400f-107">Обновление свойств объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2400f-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2400f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2400f-108">Prerequisites</span></span>
<span data-ttu-id="2400f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2400f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2400f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2400f-111">Permission type</span></span>|<span data-ttu-id="2400f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2400f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2400f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2400f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2400f-114">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="2400f-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="2400f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2400f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2400f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2400f-116">Not supported.</span></span>|
|<span data-ttu-id="2400f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2400f-117">Application</span></span>|<span data-ttu-id="2400f-118">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="2400f-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="2400f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2400f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2400f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2400f-120">Request headers</span></span>
|<span data-ttu-id="2400f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2400f-121">Header</span></span>|<span data-ttu-id="2400f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2400f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2400f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2400f-123">Authorization</span></span>|<span data-ttu-id="2400f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2400f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2400f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2400f-125">Accept</span></span>|<span data-ttu-id="2400f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2400f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2400f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2400f-127">Request body</span></span>
<span data-ttu-id="2400f-128">В тексте запроса добавьте представление объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2400f-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="2400f-129">В следующей таблице приведены свойства, необходимые при создании [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2400f-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="2400f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2400f-130">Property</span></span>|<span data-ttu-id="2400f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2400f-131">Type</span></span>|<span data-ttu-id="2400f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2400f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2400f-133">id</span><span class="sxs-lookup"><span data-stu-id="2400f-133">id</span></span>|<span data-ttu-id="2400f-134">String</span><span class="sxs-lookup"><span data-stu-id="2400f-134">String</span></span>|<span data-ttu-id="2400f-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2400f-135">Not yet documented</span></span>|
|<span data-ttu-id="2400f-136">target</span><span class="sxs-lookup"><span data-stu-id="2400f-136">target</span></span>|[<span data-ttu-id="2400f-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2400f-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="2400f-138">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="2400f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2400f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2400f-139">Response</span></span>
<span data-ttu-id="2400f-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2400f-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2400f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2400f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2400f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2400f-142">Request</span></span>
<span data-ttu-id="2400f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2400f-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2400f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2400f-144">Response</span></span>
<span data-ttu-id="2400f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2400f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



