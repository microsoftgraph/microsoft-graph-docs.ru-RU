---
title: Обновление rbacApplicationMultiple
description: Обновление свойств объекта rbacApplicationMultiple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ff5e5cfff449c305c794024f7cedeaa031f358a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148472"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="253d4-103">Обновление rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="253d4-103">Update rbacApplicationMultiple</span></span>

<span data-ttu-id="253d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="253d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="253d4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="253d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="253d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="253d4-107">Обновление свойств объекта [rbacApplicationMultiple.](../resources/intune-rbac-rbacapplicationmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="253d4-107">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="253d4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="253d4-108">Prerequisites</span></span>
<span data-ttu-id="253d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="253d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="253d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="253d4-111">Permission type</span></span>|<span data-ttu-id="253d4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="253d4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="253d4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="253d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="253d4-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="253d4-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="253d4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="253d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="253d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253d4-116">Not supported.</span></span>|
|<span data-ttu-id="253d4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="253d4-117">Application</span></span>|<span data-ttu-id="253d4-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="253d4-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="253d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="253d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="253d4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="253d4-120">Request headers</span></span>
|<span data-ttu-id="253d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="253d4-121">Header</span></span>|<span data-ttu-id="253d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="253d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="253d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="253d4-123">Authorization</span></span>|<span data-ttu-id="253d4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="253d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="253d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="253d4-125">Accept</span></span>|<span data-ttu-id="253d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="253d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="253d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="253d4-127">Request body</span></span>
<span data-ttu-id="253d4-128">В теле запроса поставляем представление JSON для объекта [rbacApplicationMultiple.](../resources/intune-rbac-rbacapplicationmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="253d4-128">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="253d4-129">В следующей таблице показаны свойства, необходимые при создании [rbacApplicationMultiple.](../resources/intune-rbac-rbacapplicationmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="253d4-129">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="253d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="253d4-130">Property</span></span>|<span data-ttu-id="253d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="253d4-131">Type</span></span>|<span data-ttu-id="253d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="253d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="253d4-133">id</span><span class="sxs-lookup"><span data-stu-id="253d4-133">id</span></span>|<span data-ttu-id="253d4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="253d4-134">String</span></span>|<span data-ttu-id="253d4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="253d4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="253d4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="253d4-136">Response</span></span>
<span data-ttu-id="253d4-137">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="253d4-137">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="253d4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="253d4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="253d4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="253d4-139">Request</span></span>
<span data-ttu-id="253d4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="253d4-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="253d4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="253d4-141">Response</span></span>
<span data-ttu-id="253d4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="253d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```




