---
title: Создание Оффицеклиентконфигуратионассигнмент
description: Добавление целевой группы в существующую политику.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e646b70ea3e18a79aaee5b4129e54da833c5c4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483826"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="69d22-103">Создание Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="69d22-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="69d22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69d22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69d22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69d22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69d22-106">Добавление целевой группы в существующую политику.</span><span class="sxs-lookup"><span data-stu-id="69d22-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69d22-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69d22-107">Prerequisites</span></span>
<span data-ttu-id="69d22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69d22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69d22-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69d22-110">Permission type</span></span>|<span data-ttu-id="69d22-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69d22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69d22-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69d22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69d22-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d22-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69d22-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69d22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69d22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69d22-115">Not supported.</span></span>|
|<span data-ttu-id="69d22-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69d22-116">Application</span></span>|<span data-ttu-id="69d22-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69d22-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69d22-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69d22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="69d22-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69d22-119">Request headers</span></span>
|<span data-ttu-id="69d22-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69d22-120">Header</span></span>|<span data-ttu-id="69d22-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69d22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69d22-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69d22-122">Authorization</span></span>|<span data-ttu-id="69d22-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69d22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69d22-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69d22-124">Accept</span></span>|<span data-ttu-id="69d22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69d22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69d22-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69d22-126">Request body</span></span>
<span data-ttu-id="69d22-127">В тексте запроса добавьте представление объекта Оффицеклиентконфигуратионассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69d22-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="69d22-128">В следующей таблице приведены свойства, необходимые при создании Оффицеклиентконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69d22-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="69d22-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69d22-129">Property</span></span>|<span data-ttu-id="69d22-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69d22-130">Type</span></span>|<span data-ttu-id="69d22-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69d22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69d22-132">id</span><span class="sxs-lookup"><span data-stu-id="69d22-132">id</span></span>|<span data-ttu-id="69d22-133">String</span><span class="sxs-lookup"><span data-stu-id="69d22-133">String</span></span>|<span data-ttu-id="69d22-134">Идентификатор объекта Оффицеконфигуратионассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69d22-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="69d22-135">target</span><span class="sxs-lookup"><span data-stu-id="69d22-135">target</span></span>|[<span data-ttu-id="69d22-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="69d22-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="69d22-137">Целевое назначение, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="69d22-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="69d22-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="69d22-138">Response</span></span>
<span data-ttu-id="69d22-139">В случае успешного выполнения этот метод возвращает `200 Created` код отклика и объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69d22-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69d22-140">Пример</span><span class="sxs-lookup"><span data-stu-id="69d22-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="69d22-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="69d22-141">Request</span></span>
<span data-ttu-id="69d22-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69d22-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69d22-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="69d22-143">Response</span></span>
<span data-ttu-id="69d22-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69d22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



