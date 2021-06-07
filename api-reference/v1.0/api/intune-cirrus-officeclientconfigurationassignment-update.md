---
title: Обновление officeClientConfigurationAssignment
description: Обновление свойств объекта officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8546e12dd6f6945240c5dc46e07f281015b3047
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753463"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="861bc-103">Обновление officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="861bc-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="861bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="861bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="861bc-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="861bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="861bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="861bc-107">Обновление свойств объекта [officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="861bc-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="861bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="861bc-108">Prerequisites</span></span>
<span data-ttu-id="861bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="861bc-111">Permission type</span></span>|<span data-ttu-id="861bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="861bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="861bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="861bc-114">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="861bc-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="861bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="861bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861bc-116">Not supported.</span></span>|
|<span data-ttu-id="861bc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="861bc-117">Application</span></span>|<span data-ttu-id="861bc-118">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="861bc-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="861bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="861bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="861bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="861bc-120">Request headers</span></span>
|<span data-ttu-id="861bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="861bc-121">Header</span></span>|<span data-ttu-id="861bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="861bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="861bc-123">Authorization</span></span>|<span data-ttu-id="861bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="861bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="861bc-125">Accept</span></span>|<span data-ttu-id="861bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="861bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="861bc-127">Request body</span></span>
<span data-ttu-id="861bc-128">В теле запроса поставляем представление JSON для [объекта officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="861bc-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="861bc-129">В следующей таблице показаны свойства, необходимые при создании [officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="861bc-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="861bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="861bc-130">Property</span></span>|<span data-ttu-id="861bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="861bc-131">Type</span></span>|<span data-ttu-id="861bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="861bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861bc-133">id</span><span class="sxs-lookup"><span data-stu-id="861bc-133">id</span></span>|<span data-ttu-id="861bc-134">String</span><span class="sxs-lookup"><span data-stu-id="861bc-134">String</span></span>|<span data-ttu-id="861bc-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="861bc-135">Not yet documented</span></span>|
|<span data-ttu-id="861bc-136">target</span><span class="sxs-lookup"><span data-stu-id="861bc-136">target</span></span>|[<span data-ttu-id="861bc-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="861bc-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="861bc-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="861bc-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="861bc-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="861bc-139">Response</span></span>
<span data-ttu-id="861bc-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="861bc-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861bc-141">Пример</span><span class="sxs-lookup"><span data-stu-id="861bc-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="861bc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="861bc-142">Request</span></span>
<span data-ttu-id="861bc-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="861bc-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="861bc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="861bc-144">Response</span></span>
<span data-ttu-id="861bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="861bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




