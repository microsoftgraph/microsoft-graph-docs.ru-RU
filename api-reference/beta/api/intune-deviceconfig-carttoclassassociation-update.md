---
title: Обновление cartToClassAssociation
description: Обновление свойств объекта cartToClassAssociation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55889fb6707c63ccae33fab28551b0bba6ba24f0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155780"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="de3bc-103">Обновление cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="de3bc-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="de3bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de3bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de3bc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de3bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de3bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de3bc-107">Обновление свойств объекта [cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)</span><span class="sxs-lookup"><span data-stu-id="de3bc-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de3bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de3bc-108">Prerequisites</span></span>
<span data-ttu-id="de3bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de3bc-111">Permission type</span></span>|<span data-ttu-id="de3bc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de3bc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de3bc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de3bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de3bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de3bc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de3bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de3bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3bc-116">Not supported.</span></span>|
|<span data-ttu-id="de3bc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de3bc-117">Application</span></span>|<span data-ttu-id="de3bc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3bc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de3bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de3bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="de3bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de3bc-120">Request headers</span></span>
|<span data-ttu-id="de3bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de3bc-121">Header</span></span>|<span data-ttu-id="de3bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de3bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de3bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3bc-123">Authorization</span></span>|<span data-ttu-id="de3bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de3bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de3bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de3bc-125">Accept</span></span>|<span data-ttu-id="de3bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de3bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de3bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de3bc-127">Request body</span></span>
<span data-ttu-id="de3bc-128">В теле запроса поставляем представление JSON для [объекта cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)</span><span class="sxs-lookup"><span data-stu-id="de3bc-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="de3bc-129">В следующей таблице показаны свойства, необходимые при создании [cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)</span><span class="sxs-lookup"><span data-stu-id="de3bc-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="de3bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de3bc-130">Property</span></span>|<span data-ttu-id="de3bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de3bc-131">Type</span></span>|<span data-ttu-id="de3bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de3bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de3bc-133">id</span><span class="sxs-lookup"><span data-stu-id="de3bc-133">id</span></span>|<span data-ttu-id="de3bc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="de3bc-134">String</span></span>|<span data-ttu-id="de3bc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="de3bc-135">Key of the entity.</span></span>|
|<span data-ttu-id="de3bc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de3bc-136">createdDateTime</span></span>|<span data-ttu-id="de3bc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de3bc-137">DateTimeOffset</span></span>|<span data-ttu-id="de3bc-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="de3bc-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="de3bc-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de3bc-139">lastModifiedDateTime</span></span>|<span data-ttu-id="de3bc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de3bc-140">DateTimeOffset</span></span>|<span data-ttu-id="de3bc-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="de3bc-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="de3bc-142">version</span><span class="sxs-lookup"><span data-stu-id="de3bc-142">version</span></span>|<span data-ttu-id="de3bc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="de3bc-143">Int32</span></span>|<span data-ttu-id="de3bc-144">Версия CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="de3bc-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="de3bc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="de3bc-145">displayName</span></span>|<span data-ttu-id="de3bc-146">Строка</span><span class="sxs-lookup"><span data-stu-id="de3bc-146">String</span></span>|<span data-ttu-id="de3bc-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="de3bc-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="de3bc-148">description</span><span class="sxs-lookup"><span data-stu-id="de3bc-148">description</span></span>|<span data-ttu-id="de3bc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="de3bc-149">String</span></span>|<span data-ttu-id="de3bc-150">Администратор предоставил описание CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="de3bc-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="de3bc-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="de3bc-151">deviceCartIds</span></span>|<span data-ttu-id="de3bc-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de3bc-152">String collection</span></span>|<span data-ttu-id="de3bc-153">Идентификаторы тележек устройств, связанных с классами.</span><span class="sxs-lookup"><span data-stu-id="de3bc-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="de3bc-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="de3bc-154">classroomIds</span></span>|<span data-ttu-id="de3bc-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de3bc-155">String collection</span></span>|<span data-ttu-id="de3bc-156">Идентификаторы классов, связанных с тележками устройств.</span><span class="sxs-lookup"><span data-stu-id="de3bc-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="de3bc-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3bc-157">Response</span></span>
<span data-ttu-id="de3bc-158">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de3bc-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de3bc-159">Пример</span><span class="sxs-lookup"><span data-stu-id="de3bc-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="de3bc-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="de3bc-160">Request</span></span>
<span data-ttu-id="de3bc-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de3bc-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="de3bc-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3bc-162">Response</span></span>
<span data-ttu-id="de3bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de3bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```




