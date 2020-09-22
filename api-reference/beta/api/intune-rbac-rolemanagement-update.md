---
title: Обновление Ролеманажемент
description: Обновление свойств объекта Ролеманажемент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0aeff280e468dd672ba747de034f278f8226ba2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072069"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="503c7-103">Обновление Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="503c7-103">Update roleManagement</span></span>

<span data-ttu-id="503c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="503c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="503c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503c7-107">Обновление свойств объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="503c7-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="503c7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="503c7-108">Prerequisites</span></span>
<span data-ttu-id="503c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="503c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="503c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="503c7-111">Permission type</span></span>|<span data-ttu-id="503c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="503c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="503c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="503c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="503c7-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503c7-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="503c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="503c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="503c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503c7-116">Not supported.</span></span>|
|<span data-ttu-id="503c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="503c7-117">Application</span></span>|<span data-ttu-id="503c7-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503c7-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="503c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="503c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="503c7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="503c7-120">Request headers</span></span>
|<span data-ttu-id="503c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="503c7-121">Header</span></span>|<span data-ttu-id="503c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="503c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="503c7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="503c7-123">Authorization</span></span>|<span data-ttu-id="503c7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="503c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="503c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="503c7-125">Accept</span></span>|<span data-ttu-id="503c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="503c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="503c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="503c7-127">Request body</span></span>
<span data-ttu-id="503c7-128">В тексте запроса добавьте представление объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="503c7-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="503c7-129">В следующей таблице приведены свойства, необходимые при создании [ролеманажемент](../resources/intune-rbac-rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="503c7-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="503c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="503c7-130">Property</span></span>|<span data-ttu-id="503c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="503c7-131">Type</span></span>|<span data-ttu-id="503c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="503c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503c7-133">id</span><span class="sxs-lookup"><span data-stu-id="503c7-133">id</span></span>|<span data-ttu-id="503c7-134">String</span><span class="sxs-lookup"><span data-stu-id="503c7-134">String</span></span>|<span data-ttu-id="503c7-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="503c7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="503c7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="503c7-136">Response</span></span>
<span data-ttu-id="503c7-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролеманажемент](../resources/intune-rbac-rolemanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="503c7-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="503c7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="503c7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="503c7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="503c7-139">Request</span></span>
<span data-ttu-id="503c7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="503c7-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="503c7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="503c7-141">Response</span></span>
<span data-ttu-id="503c7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="503c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```






