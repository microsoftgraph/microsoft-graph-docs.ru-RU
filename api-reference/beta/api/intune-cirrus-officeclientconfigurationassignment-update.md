---
title: Обновление officeClientConfigurationAssignment
description: Обновление свойств объекта officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8546e12dd6f6945240c5dc46e07f281015b3047
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666054"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="802ca-103">Обновление officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="802ca-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="802ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="802ca-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="802ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="802ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="802ca-107">Обновление свойств объекта [officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="802ca-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="802ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="802ca-108">Prerequisites</span></span>
<span data-ttu-id="802ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="802ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="802ca-111">Permission type</span></span>|<span data-ttu-id="802ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="802ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="802ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="802ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="802ca-114">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="802ca-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="802ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="802ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="802ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802ca-116">Not supported.</span></span>|
|<span data-ttu-id="802ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="802ca-117">Application</span></span>|<span data-ttu-id="802ca-118">\*\*TODO: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="802ca-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="802ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="802ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="802ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="802ca-120">Request headers</span></span>
|<span data-ttu-id="802ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="802ca-121">Header</span></span>|<span data-ttu-id="802ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="802ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="802ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="802ca-123">Authorization</span></span>|<span data-ttu-id="802ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="802ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="802ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="802ca-125">Accept</span></span>|<span data-ttu-id="802ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="802ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="802ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="802ca-127">Request body</span></span>
<span data-ttu-id="802ca-128">В теле запроса поставляем представление JSON для [объекта officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="802ca-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="802ca-129">В следующей таблице показаны свойства, необходимые при создании [officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="802ca-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="802ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="802ca-130">Property</span></span>|<span data-ttu-id="802ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="802ca-131">Type</span></span>|<span data-ttu-id="802ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="802ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="802ca-133">id</span><span class="sxs-lookup"><span data-stu-id="802ca-133">id</span></span>|<span data-ttu-id="802ca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="802ca-134">String</span></span>|<span data-ttu-id="802ca-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="802ca-135">Not yet documented</span></span>|
|<span data-ttu-id="802ca-136">target</span><span class="sxs-lookup"><span data-stu-id="802ca-136">target</span></span>|[<span data-ttu-id="802ca-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="802ca-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="802ca-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="802ca-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="802ca-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="802ca-139">Response</span></span>
<span data-ttu-id="802ca-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="802ca-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802ca-141">Пример</span><span class="sxs-lookup"><span data-stu-id="802ca-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="802ca-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="802ca-142">Request</span></span>
<span data-ttu-id="802ca-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="802ca-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="802ca-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="802ca-144">Response</span></span>
<span data-ttu-id="802ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="802ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




