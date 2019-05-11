---
title: Создание Оффицеклиентконфигуратионассигнмент
description: Добавление целевой группы в существующую политику.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: e1222a23112356b1681f1cdc01556800ffe44586
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934063"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="77906-103">Создание Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="77906-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="77906-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77906-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77906-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77906-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77906-106">Добавление целевой группы в существующую политику.</span><span class="sxs-lookup"><span data-stu-id="77906-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77906-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77906-107">Prerequisites</span></span>
<span data-ttu-id="77906-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77906-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77906-110">Permission type</span></span>|<span data-ttu-id="77906-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77906-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77906-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77906-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77906-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77906-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77906-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77906-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77906-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77906-115">Not supported.</span></span>|
|<span data-ttu-id="77906-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77906-116">Application</span></span>|<span data-ttu-id="77906-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77906-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77906-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77906-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="77906-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77906-119">Request headers</span></span>
|<span data-ttu-id="77906-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77906-120">Header</span></span>|<span data-ttu-id="77906-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77906-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77906-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77906-122">Authorization</span></span>|<span data-ttu-id="77906-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77906-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77906-124">Accept</span><span class="sxs-lookup"><span data-stu-id="77906-124">Accept</span></span>|<span data-ttu-id="77906-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77906-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77906-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77906-126">Request body</span></span>
<span data-ttu-id="77906-127">В тексте запроса добавьте представление объекта Оффицеклиентконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77906-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="77906-128">В следующей таблице приведены свойства, необходимые при создании Оффицеклиентконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="77906-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="77906-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77906-129">Property</span></span>|<span data-ttu-id="77906-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77906-130">Type</span></span>|<span data-ttu-id="77906-131">Описание</span><span class="sxs-lookup"><span data-stu-id="77906-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77906-132">id</span><span class="sxs-lookup"><span data-stu-id="77906-132">id</span></span>|<span data-ttu-id="77906-133">Строка</span><span class="sxs-lookup"><span data-stu-id="77906-133">String</span></span>|<span data-ttu-id="77906-134">Идентификатор объекта Оффицеконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="77906-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="77906-135">target</span><span class="sxs-lookup"><span data-stu-id="77906-135">target</span></span>|[<span data-ttu-id="77906-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="77906-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="77906-137">Целевое назначение, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="77906-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="77906-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="77906-138">Response</span></span>
<span data-ttu-id="77906-139">В случае успешного выполнения этот метод возвращает `200 Created` код отклика и объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77906-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77906-140">Пример</span><span class="sxs-lookup"><span data-stu-id="77906-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="77906-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="77906-141">Request</span></span>
<span data-ttu-id="77906-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77906-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="77906-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="77906-143">Response</span></span>
<span data-ttu-id="77906-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77906-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



