---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66448222ab82776a343296f6bec0be0e9d684852
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025829"
---
# <a name="update-reportroot"></a><span data-ttu-id="8662d-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="8662d-103">Update reportRoot</span></span>

> <span data-ttu-id="8662d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8662d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8662d-105">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="8662d-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8662d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8662d-106">Prerequisites</span></span>
<span data-ttu-id="8662d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8662d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8662d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8662d-109">Permission type</span></span>|<span data-ttu-id="8662d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8662d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8662d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8662d-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8662d-112">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="8662d-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="8662d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8662d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8662d-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="8662d-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="8662d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8662d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8662d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8662d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8662d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8662d-117">Not supported.</span></span>|
|<span data-ttu-id="8662d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8662d-118">Application</span></span>|<span data-ttu-id="8662d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8662d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8662d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8662d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="8662d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8662d-121">Request headers</span></span>
|<span data-ttu-id="8662d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8662d-122">Header</span></span>|<span data-ttu-id="8662d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8662d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8662d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8662d-124">Authorization</span></span>|<span data-ttu-id="8662d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8662d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8662d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8662d-126">Accept</span></span>|<span data-ttu-id="8662d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8662d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8662d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8662d-128">Request body</span></span>
<span data-ttu-id="8662d-129">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8662d-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="8662d-130">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="8662d-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="8662d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8662d-131">Property</span></span>|<span data-ttu-id="8662d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8662d-132">Type</span></span>|<span data-ttu-id="8662d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8662d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8662d-134">id</span><span class="sxs-lookup"><span data-stu-id="8662d-134">id</span></span>|<span data-ttu-id="8662d-135">String</span><span class="sxs-lookup"><span data-stu-id="8662d-135">String</span></span>|<span data-ttu-id="8662d-136">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="8662d-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8662d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8662d-137">Response</span></span>
<span data-ttu-id="8662d-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8662d-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8662d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8662d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="8662d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8662d-140">Request</span></span>
<span data-ttu-id="8662d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8662d-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8662d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8662d-142">Response</span></span>
<span data-ttu-id="8662d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8662d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








