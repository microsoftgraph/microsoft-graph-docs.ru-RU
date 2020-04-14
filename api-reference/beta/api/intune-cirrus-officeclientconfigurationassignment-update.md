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
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="f5b3b-103">Обновление Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="f5b3b-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="f5b3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5b3b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5b3b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b3b-107">Обновление свойств объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f5b3b-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5b3b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5b3b-108">Prerequisites</span></span>
<span data-ttu-id="f5b3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b3b-111">Permission type</span></span>|<span data-ttu-id="f5b3b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5b3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5b3b-114">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="f5b3b-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="f5b3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5b3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-116">Not supported.</span></span>|
|<span data-ttu-id="f5b3b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5b3b-117">Application</span></span>|<span data-ttu-id="f5b3b-118">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="f5b3b-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5b3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f5b3b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5b3b-120">Request headers</span></span>
|<span data-ttu-id="f5b3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5b3b-121">Header</span></span>|<span data-ttu-id="f5b3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f5b3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5b3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b3b-123">Authorization</span></span>|<span data-ttu-id="f5b3b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5b3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5b3b-125">Accept</span></span>|<span data-ttu-id="f5b3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5b3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5b3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5b3b-127">Request body</span></span>
<span data-ttu-id="f5b3b-128">В тексте запроса добавьте представление объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="f5b3b-129">В следующей таблице приведены свойства, необходимые при создании [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f5b3b-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="f5b3b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5b3b-130">Property</span></span>|<span data-ttu-id="f5b3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b3b-131">Type</span></span>|<span data-ttu-id="f5b3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b3b-133">id</span><span class="sxs-lookup"><span data-stu-id="f5b3b-133">id</span></span>|<span data-ttu-id="f5b3b-134">String</span><span class="sxs-lookup"><span data-stu-id="f5b3b-134">String</span></span>|<span data-ttu-id="f5b3b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-135">Not yet documented</span></span>|
|<span data-ttu-id="f5b3b-136">target</span><span class="sxs-lookup"><span data-stu-id="f5b3b-136">target</span></span>|[<span data-ttu-id="f5b3b-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f5b3b-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="f5b3b-138">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="f5b3b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f5b3b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5b3b-139">Response</span></span>
<span data-ttu-id="f5b3b-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5b3b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f5b3b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5b3b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b3b-142">Request</span></span>
<span data-ttu-id="f5b3b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5b3b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b3b-144">Response</span></span>
<span data-ttu-id="f5b3b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5b3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



