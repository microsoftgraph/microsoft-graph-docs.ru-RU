---
title: Обновление Оффицеклиентконфигуратионассигнмент
description: Обновление свойств объекта Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 80b748ddff1926d0f2794c7fc9d65cde05e5faa2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934042"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="2dcf7-103">Обновление Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="2dcf7-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="2dcf7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dcf7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dcf7-106">Обновление свойств объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2dcf7-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dcf7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2dcf7-107">Prerequisites</span></span>
<span data-ttu-id="2dcf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dcf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dcf7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dcf7-110">Permission type</span></span>|<span data-ttu-id="2dcf7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dcf7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dcf7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dcf7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2dcf7-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="2dcf7-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="2dcf7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dcf7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dcf7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-115">Not supported.</span></span>|
|<span data-ttu-id="2dcf7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dcf7-116">Application</span></span>|<span data-ttu-id="2dcf7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dcf7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dcf7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2dcf7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2dcf7-119">Request headers</span></span>
|<span data-ttu-id="2dcf7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2dcf7-120">Header</span></span>|<span data-ttu-id="2dcf7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2dcf7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dcf7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dcf7-122">Authorization</span></span>|<span data-ttu-id="2dcf7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dcf7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2dcf7-124">Accept</span></span>|<span data-ttu-id="2dcf7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2dcf7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dcf7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2dcf7-126">Request body</span></span>
<span data-ttu-id="2dcf7-127">В тексте запроса добавьте представление объекта [Оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="2dcf7-128">В следующей таблице приведены свойства, необходимые при создании [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2dcf7-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="2dcf7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dcf7-129">Property</span></span>|<span data-ttu-id="2dcf7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2dcf7-130">Type</span></span>|<span data-ttu-id="2dcf7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2dcf7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dcf7-132">id</span><span class="sxs-lookup"><span data-stu-id="2dcf7-132">id</span></span>|<span data-ttu-id="2dcf7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2dcf7-133">String</span></span>|<span data-ttu-id="2dcf7-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-134">Not yet documented</span></span>|
|<span data-ttu-id="2dcf7-135">target</span><span class="sxs-lookup"><span data-stu-id="2dcf7-135">target</span></span>|[<span data-ttu-id="2dcf7-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2dcf7-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="2dcf7-137">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="2dcf7-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2dcf7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="2dcf7-138">Response</span></span>
<span data-ttu-id="2dcf7-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dcf7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2dcf7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dcf7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dcf7-141">Request</span></span>
<span data-ttu-id="2dcf7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2dcf7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dcf7-143">Response</span></span>
<span data-ttu-id="2dcf7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2dcf7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



