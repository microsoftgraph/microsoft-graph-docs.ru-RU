---
title: Обновление roleManagement
description: Обновление свойств объекта roleManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 549d3ab5bc3e4d248ba81bf5c0059a6fcd0d5e90
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156676"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="d2fc8-103">Обновление roleManagement</span><span class="sxs-lookup"><span data-stu-id="d2fc8-103">Update roleManagement</span></span>

<span data-ttu-id="d2fc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2fc8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2fc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2fc8-107">Обновление свойств объекта [roleManagement.](../resources/intune-rbac-rolemanagement.md)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2fc8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2fc8-108">Prerequisites</span></span>
<span data-ttu-id="d2fc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2fc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2fc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2fc8-111">Permission type</span></span>|<span data-ttu-id="d2fc8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2fc8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2fc8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2fc8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d2fc8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2fc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-116">Not supported.</span></span>|
|<span data-ttu-id="d2fc8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2fc8-117">Application</span></span>|<span data-ttu-id="d2fc8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2fc8-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2fc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2fc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="d2fc8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2fc8-120">Request headers</span></span>
|<span data-ttu-id="d2fc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2fc8-121">Header</span></span>|<span data-ttu-id="d2fc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2fc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2fc8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2fc8-123">Authorization</span></span>|<span data-ttu-id="d2fc8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2fc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2fc8-125">Accept</span></span>|<span data-ttu-id="d2fc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2fc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2fc8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2fc8-127">Request body</span></span>
<span data-ttu-id="d2fc8-128">В теле запроса поставляем представление JSON для [объекта roleManagement.](../resources/intune-rbac-rolemanagement.md)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="d2fc8-129">В следующей таблице показаны свойства, необходимые при создании [roleManagement.](../resources/intune-rbac-rolemanagement.md)</span><span class="sxs-lookup"><span data-stu-id="d2fc8-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="d2fc8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2fc8-130">Property</span></span>|<span data-ttu-id="d2fc8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d2fc8-131">Type</span></span>|<span data-ttu-id="d2fc8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d2fc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2fc8-133">id</span><span class="sxs-lookup"><span data-stu-id="d2fc8-133">id</span></span>|<span data-ttu-id="d2fc8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d2fc8-134">String</span></span>|<span data-ttu-id="d2fc8-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2fc8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2fc8-136">Response</span></span>
<span data-ttu-id="d2fc8-137">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [roleManagement](../resources/intune-rbac-rolemanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2fc8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d2fc8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2fc8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2fc8-139">Request</span></span>
<span data-ttu-id="d2fc8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="d2fc8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2fc8-141">Response</span></span>
<span data-ttu-id="d2fc8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2fc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```




