---
title: Создание Оффицеклиентконфигуратионассигнмент
description: Добавление целевой группы в существующую политику.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e9517ee0937146a7e05b016d5f58a49236ca229
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392010"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="75ef1-103">Создание Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="75ef1-103">Create officeClientConfigurationAssignment</span></span>

<span data-ttu-id="75ef1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ef1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75ef1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ef1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75ef1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75ef1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ef1-107">Добавление целевой группы в существующую политику.</span><span class="sxs-lookup"><span data-stu-id="75ef1-107">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75ef1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75ef1-108">Prerequisites</span></span>
<span data-ttu-id="75ef1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ef1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75ef1-111">Permission type</span></span>|<span data-ttu-id="75ef1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75ef1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75ef1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75ef1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75ef1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ef1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75ef1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75ef1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75ef1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ef1-116">Not supported.</span></span>|
|<span data-ttu-id="75ef1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75ef1-117">Application</span></span>|<span data-ttu-id="75ef1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ef1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75ef1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75ef1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="75ef1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75ef1-120">Request headers</span></span>
|<span data-ttu-id="75ef1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75ef1-121">Header</span></span>|<span data-ttu-id="75ef1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75ef1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75ef1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75ef1-123">Authorization</span></span>|<span data-ttu-id="75ef1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75ef1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75ef1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75ef1-125">Accept</span></span>|<span data-ttu-id="75ef1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75ef1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ef1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75ef1-127">Request body</span></span>
<span data-ttu-id="75ef1-128">В тексте запроса добавьте представление объекта Оффицеклиентконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75ef1-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="75ef1-129">В следующей таблице приведены свойства, необходимые при создании Оффицеклиентконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="75ef1-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="75ef1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75ef1-130">Property</span></span>|<span data-ttu-id="75ef1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75ef1-131">Type</span></span>|<span data-ttu-id="75ef1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75ef1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ef1-133">id</span><span class="sxs-lookup"><span data-stu-id="75ef1-133">id</span></span>|<span data-ttu-id="75ef1-134">String</span><span class="sxs-lookup"><span data-stu-id="75ef1-134">String</span></span>|<span data-ttu-id="75ef1-135">Идентификатор объекта Оффицеконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="75ef1-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="75ef1-136">target</span><span class="sxs-lookup"><span data-stu-id="75ef1-136">target</span></span>|[<span data-ttu-id="75ef1-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="75ef1-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="75ef1-138">Целевое назначение, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="75ef1-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="75ef1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="75ef1-139">Response</span></span>
<span data-ttu-id="75ef1-140">В случае успешного выполнения этот метод возвращает `200 Created` код отклика и объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75ef1-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75ef1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="75ef1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="75ef1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="75ef1-142">Request</span></span>
<span data-ttu-id="75ef1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75ef1-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75ef1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ef1-144">Response</span></span>
<span data-ttu-id="75ef1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75ef1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



