---
title: Создание Оффицеклиентконфигуратионассигнмент
description: Добавление целевой группы в существующую политику.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3833115c1b652794e8d6b0557824389ebb974dd2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170861"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="f71bd-103">Создание Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="f71bd-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="f71bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f71bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f71bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f71bd-106">Добавление целевой группы в существующую политику.</span><span class="sxs-lookup"><span data-stu-id="f71bd-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f71bd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f71bd-107">Prerequisites</span></span>
<span data-ttu-id="f71bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f71bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f71bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f71bd-110">Permission type</span></span>|<span data-ttu-id="f71bd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f71bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f71bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f71bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f71bd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f71bd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f71bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f71bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f71bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71bd-115">Not supported.</span></span>|
|<span data-ttu-id="f71bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f71bd-116">Application</span></span>|<span data-ttu-id="f71bd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f71bd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f71bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f71bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f71bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f71bd-119">Request headers</span></span>
|<span data-ttu-id="f71bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f71bd-120">Header</span></span>|<span data-ttu-id="f71bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f71bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f71bd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f71bd-122">Authorization</span></span>|<span data-ttu-id="f71bd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f71bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f71bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f71bd-124">Accept</span></span>|<span data-ttu-id="f71bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f71bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f71bd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f71bd-126">Request body</span></span>
<span data-ttu-id="f71bd-127">В тексте запроса добавьте представление объекта Оффицеклиентконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f71bd-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="f71bd-128">В следующей таблице приведены свойства, необходимые при создании Оффицеклиентконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="f71bd-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="f71bd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f71bd-129">Property</span></span>|<span data-ttu-id="f71bd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f71bd-130">Type</span></span>|<span data-ttu-id="f71bd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f71bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f71bd-132">id</span><span class="sxs-lookup"><span data-stu-id="f71bd-132">id</span></span>|<span data-ttu-id="f71bd-133">String</span><span class="sxs-lookup"><span data-stu-id="f71bd-133">String</span></span>|<span data-ttu-id="f71bd-134">Идентификатор объекта Оффицеконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="f71bd-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="f71bd-135">target</span><span class="sxs-lookup"><span data-stu-id="f71bd-135">target</span></span>|[<span data-ttu-id="f71bd-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f71bd-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="f71bd-137">Целевое назначение, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="f71bd-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f71bd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71bd-138">Response</span></span>
<span data-ttu-id="f71bd-139">В случае успешного выполнения этот метод возвращает `200 Created` код отклика и объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f71bd-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f71bd-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f71bd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f71bd-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f71bd-141">Request</span></span>
<span data-ttu-id="f71bd-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f71bd-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f71bd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71bd-143">Response</span></span>
<span data-ttu-id="f71bd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f71bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




